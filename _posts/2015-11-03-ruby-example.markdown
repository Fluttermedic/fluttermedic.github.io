---
layout: post
title:  "Ruby example"
date:   2015-11-03 17:28:36 -0600
categories: example
---

So. Here's our code!

{% highlight ruby %}
array = [5, 4, 3, 2, 1] =begin This is a variable that's equal to an array.
 An array is, well, an array of numbers or text.
 =end
array.sort!  =begin Sort causes things to be sorted out alphanumerically.
The exclamation mark forces the code itself
to be changed when Sort is called on it.
=end
puts array =begin
Puts is short for put string, and a string is text or numbers or words,
put each on their own line.  
=end
print array  #Print would print everything out, like puts, except it does it all in one line. 

=begin
When calling the previous puts and print, it's saying
to put out into text whatever is in the array variable
=end
array2 = ["e", "d", "c", "b", "a"] #Even works alphabetically.
array2.sort!

puts array2
print array2

#Oh. These little comments that are preceeded by the pound sign? They're only here for people reading the codes.
{% endhighlight %}

So. Here's what our output looks like.

1
2
3
4
5
[1, 2, 3, 4, 5]a
b
c
d
e
["a", "b", "c", "d", "e"]


The reason that is, is because first I'm `puts`ing it, every number and letter is in its own line.
Then it's shown in its own `array`, though I probably could have spaced it out. Oh well.
Letters have to be part of a `string`, otherwise they're seen as unassigned variables. So a `string` can even be a single character.

And if you noticed, our code had these in the reverse order, until we called the `.sort!` command to force the output to come out in the correct order, and, also, it changed the code after it hit the `!`, instead of just changing what the output looked like.