---
title: Down the Rabbit Hole
date: 2018-03-29
tags: code, blockers, different, refactor, mentoring
---

# Down the Rabbit Hole.

> “But I don’t want to go among mad people," Alice remarked.
> "Oh, you can’t help that," said the Cat: "we’re all mad here. I’m mad. You’re mad."
> "How do you know I’m mad?" said Alice.
> "You must be," said the Cat, "or you wouldn’t have come here.”
> ― Lewis Carroll, Alice in Wonderland

### Through the Looking Glass

![rabbit hole](https://images.pexels.com/photos/121663/pexels-photo-121663.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260)

This week I met up with [Joseph Hawkins](https://github.com/chinamisr254){:target="_blank"} a budding Ruby Developer from the US who I helped a little to find his way out of a rabbit hole in his code.

For me, when I'm mentoring folks I find it interesting to see how folks are taught programming in different countries but with similar code assignments. And it's interesting to meet different people who learn at different speeds and do different things to solve the same problem.

As some people might know, I've been mentoring my sister [Sophie McDonald](https://twitter.com/sophierose239){:target="_blank"} as well and one thing I find about mentoring is that I usually get asked similar questions. So I thought I should write something so that people who are aspiring to be programmers understand that even programmers who you think are "so above you" actually make mistakes and can get into similar situations like you too.

And the reason I say this is because we all have similar fears and anxiety around learning something new or even old.

<blockquote class="twitter-tweet" data-lang="en-gb"><p lang="en" dir="ltr">I have been coding Ruby for over a decade and yet I just lost an hour because of something expecting a string when I was giving it a symbol.</p>&mdash; Ryan Bigg (@ryanbigg) <a href="https://twitter.com/ryanbigg/status/979578016127885312?ref_src=twsrc%5Etfw">30 March 2018</a></blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

<br>

### Brainfarts and Rabbit Holes

I'm a little embarrassed to admit this but I have "brainfarts" moments all the time and end up in rabbit holes so much so that I can end up wasting time writing silly code that is not even needed. Usually it happens when I'm stressed or I haven't had enough sleep or even from just the weather being awful.

So if it's really important to make sure your mental health and physical health is in tip top shape if you want to function properly.

Ok.. soooo here is the problem I spent a bunch of time on that is really embarrassing for me.

I had an input field similar to the one below with:

```
<select class="form-control" name="language" type="language" id="language">
  <option value="">Select Language</option>
  <option value="1">English</option>
  <option value="2">French</option>
  <option value="3">Japanese</option>
</select>
```

<select class="form-control" name="language" type="language" id="language">
  <option value="">Select Language</option>
  <option value="1">English</option>
  <option value="2">French</option>
  <option value="3">Japanese</option>
</select>

And for some reason I couldn't remember that you there is an ability to have a `selected` option in html.

So I started writing in Python a way to remove the language I was selecting from the list because it would showing up twice the way I had written the HTML originally. I had even spent some time writing tests to solve this. 😨

The messed up way looked like the following:

<select class="form-control" name="language" type="language" id="language">
  <option value="3">Japanese</option>
  <option value="1">English</option>
  <option value="2">French</option>
  <option value="3">Japanese</option>
</select>

Seriously, open that drop down menu up and see what's going on and you'll see the issue I had. 😅 And I was trying to solve this problem in the backend with Python. WTF brain why aren't you working?!?!

Anyway, after a day or something and talking with a workmate, 🦆 I realised that all I needed to do was write the following:

`<option value="3" selected>Japanese</option>`

So that it would turn out like this:

<select class="form-control" name="language" type="language" id="language">
  <option value="">Select Language</option>
  <option value="1">English</option>
  <option value="2">French</option>
  <option value="3" selected>Japanese</option>
</select>

I'm not even going to show you the Python I wrote for trying to solve this problem because no one should see that EVER. And also it's completely useless so if I put it anywhere I'm worried people might use it.

It's been deleted forever now.

### Fear of Failure

![fear](https://images.pexels.com/photos/568027/pexels-photo-568027.jpeg?auto=compress&cs=tinysrgb&h=650&w=940)

I feel like a lot of questions on Stack Overflow, especially Javascript problems, are people having brainfart moments. I think it's important that those exist but sometimes they can lead us down the wrong path and we end up losing our way.

So if you do post on Stack Overflow (and I highly recommend you do at some stage) make sure you have tried to researched the problem thoroughly and checked to see if someone has asked a similar question. Believe me when I say, there is most likely an answer already written somewhere about the same problem.

*Overcome the fear of failure because the first step to success is to at least try.*

And don't feel bad if you don't know something. Just Google it! Even if you feel it's something you should already know. Learning something over and over again is calling practicing and it helps you become better by committing it to your long term memory.

Basically what I'm trying to say with this post, is that everyone has these moments even people who have been coding for years. So if you are ever feeling like you can't do it just remember we are all have the ability to do it wrong.
