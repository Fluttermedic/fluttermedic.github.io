---
layout: post
title:  "Exercism stuff!"
date:   2015-11-03 17:28:36 -0600
categories: exercism
---

So our first little excercise is pretty simple, all things considered. Still got help with it, of course, as I'm a newbie.

This is the solution we (Rubygeek) came up with after a bit of experimenting. 

```ruby
class HelloWorld
  def self.hello(name = "World")
    "Hello, #{name}!"
  end
end
```

It's about the shortest that we could figure it. We went through a couple of them, but that's the last one we ran with.

The problem, by the way, would be this. Kind of important to know the problem I guess.

The Readme http://exercism.io/exercises/ruby/hello-world/readme
The test itself. http://exercism.io/exercises/ruby/hello-world


The second one, I, of course, had quite a bit of help with as well. But apparently I was close to having the right idea.

I wanted to get a `loop` going that would count up the differences counter with each new difference, using the `until` command. After attempting to articulate it, we eventually were able to come up with this for the second test.

```ruby 
class Hamming
  def self.compute(a, b)
    alength = a.length
    
    blength = b.length
    
    if alength != blength
      
      raise ArgumentError
      
    end
     
    differences = 0
    
    0.upto(alength) do |idx|
      
      if a[idx] != b[idx]
        
        differences += 1
        
      end
      
    end
      
    differences
    
  end
  
end
```

Using `.upto`, the numbers would count up along the differences, into the differences value, from 0, to the appropriate number. The differences were coming up between the arguments' character values. As in, how many different values were there between, say (ABCAAA, ABCVSC). In the cases were the values were not equal such as in (AAA, ABCD) we had to call the `raise` `ArgumentError` command.

Readme http://exercism.io/exercises/ruby/hamming/readme
Test http://exercism.io/exercises/ruby/hamming