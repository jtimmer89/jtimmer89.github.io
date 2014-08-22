---
layout: post
title: "Technical Blog: Looping in Ruby"
quote: When you realize that looping isn't something that only a hula hoop does.
image: /media/technical-blogs/AutumnLake_14.jpg
video: false
---

#Ways to Loop in Ruby

Compared to our work with javascript last week, Ruby offers numerous ways of looping for different circumstances. The different loop statements include the following: times, each, for, while, until, do/break if, and upto. I’m sure I missed some ways as there are many ways to loop or iterate in Ruby. Let’s take a look at the different ways I mentioned.

####Times

Times does a simple looping any number of times.

```
  10.times
  puts “Joe Timmer is real neat”
  end
```
####Each

Times does a simple looping any number of times.

```
  cats = [“Marty”, “Harry”, “Samantha”]
  cats.each { |names| puts names + “-cat” }
```

####For

The for loop is also used in javascript but it has a different syntax in Ruby.

```
  for i in 1..10
    puts “Joe Timmer is real neat”
  end
```

####While

The while loop does a block of code while a certain condition is true.

```
  i = 0
  while i < 10
    puts “Joe Timmer is real neat”
    i += 1
  end
```

####Until

The until loop starts to make you think. It does a block of code until something is true, like a backwards while loop.

```
  i = 1
  until i > 10
    puts “Joe Timmer is real neat”
    i += 1
  end
```

####Do/Break

The do/break if loop allows you to do something and stop doing it if a condition is true.

```
  i = 1
  loop do
    puts “Joe Timmer is real neat”
    i += 1
  break if i > 10
  end
```

####Upto

The final loop that I want to look at is a simple one. Upto. It basically does a block of code from one number up to another number times.

```
  1.upto(10) do
    puts “Joe Timmer is real neat”
  end
```

##How to decide which loop to use

There are many ways to use these different loops other than the basic syntax that I gave in the examples, but how do you decide which to use given the challenge you are working on? I had a hard time finding many resources on which loop is best so this will basically be from my own noggin. I look for readability. What makes sense if you were writing the code as an English sentence? This can help you decide which keyword to use. Also, how many lines can you do the code in? The less, the better. Finally, how is the computer processing the code? You want your code to be readable, concise, and fast. I would consider these three factors when looking at which keyword to use. Does is sound good? Does another loop allow for less code? The third one is a bit more complex and will probably take time to really consider after learning how each keyword works more fully.