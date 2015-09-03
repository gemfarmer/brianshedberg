---
layout: page
permalink: /errors/
---

###JS:

{% highlight javascript%}
try{
	something();
} catch{
	doSomethingElse();	
}{% endhighlight %}

###Python

{% highlight python%}
try:
	something()
except ValueError:
	do_something_else(){% endhighlight %}

In the above python example, the error is only caught if there is a ValueError, a different kind of error could also be made an exception

[List of Python Exceptions](https://docs.python.org/2/library/exceptions.html)