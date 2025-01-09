---
layout: post
title: Book review on Python Distilled
---

<div class="message">
  Python Distilled is written by David M. Beazley in 2021. Here's the Amazon link to this book:
  https://www.amazon.com/Python-Essential-Reference-Developers-Library/dp/0134173279
</div>

As an engineer who regularly will use Python for daily job, I was looking for a book which could help me move from a Python beginner to intermediate Python developer. Such topics includes but not limited to the following: 

- how to understand Objects deeply 
- what are the meanings of different arguments types
- how to do error handling, what is Decorator
- what is Generator
- what is lambda Expression
- how to better under Modules and Packages
- how to do complex Input and Output

Yes, many of those topics have been addressed by some excellent YouTube videos such as [Corey Schafer](https://www.youtube.com/@coreyms), but they are not systematically, at least for myself. So I did a lot of Googling as well as reading Amazon reviews to find the book could satisfy my needs. According to my investigation, those candidates are:

- [Pydon'ts – Write elegant Python code](https://mathspp.com/books/pydonts?utm_source=insider.mathspp.com&utm_medium=newsletter&utm_campaign=simplifying-nested-loops-with-generators)
- [Beyond the Basic Stuff with Python](https://inventwithpython.com/beyond/)
- [Intermediate Python](https://leanpub.com/intermediatepython)
- [Python Cookbook: Recipes for Mastering Python 3](https://www.amazon.com/Python-Cookbook-Third-David-Beazley/dp/1449340377/ref=as_li_ss_tl?ie=UTF8&qid=1437328145&sr=8-1&keywords=python+cookbook&linkCode=sl1&tag=ththfrthmo00-20&linkId=babc3a4c6b83554ab19975b4d15e06c5)
- [Fluent Python: Clear, Concise, and Effective Programming](https://www.amazon.com/Fluent-Python-Concise-Effective-Programming/dp/1491946008)

Some of those authors are very good, they provided free e-books. Some of them have the contents for what I need, but they are very thick such as Python Cookbook and Fluent Python. What I need is a book which can also cover all those important topics while not too length so I could finish it :) After some extensive researches, I finally landed my eyes on this book Python Distilled. For me, it covers all the important topics I need while keep its lenthy not too scary.

And this book didn't disappoint me. It does cover all the topics I really concern. And indeed as its name, this book controls its ilustration as dry as possible, but still have good examples so the readers can understand those concepts. For example, here's the explanation for First-Class Objects:

<div class="message">
  All objects in Python are said to be first-class. This means that all objects that can be assigned to a name can also be treated as data. As data, objects can be stored as variables, passed as arguments, returned from fuctions, compared against other objects, and more. 
</div>

Then the author gave a short but good example:

{% highlight js %}
// For example, here is a simple dictionary containing two values:

items = {
    'number' : 42
    'text' : "Hello World"
}

// The first-class nature of objects can be seen by adding some more unusual items to this dictionary:
items['func'] = abs
import math
items['mod'] = math

{% endhighlight %}

Another thing I like this book is that in the last chapter Chapter 10, it provides all the Python Build-in Functions, all built-in Exceptions and all Python Standard Libraries so far. This can be used as dictionary or reference and gives the readers who are new to Python a general picture of all the tools we can use. After getting more familiar with those fundamental tools, new Python users will easier to move to the other tools as well.

### Some errors
This is a great book, but I also found some errors from it. 

In page 250, Section 9.3, the author gave the following example:
> format(x, '<*10.2f>')    # '123.46****'
The correct form should be:
format(x, '*<10.2f>')
