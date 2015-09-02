---
layout: page
title: Lists
permalink: /lists/
---

In python, lists are mutable and can be changed
{% highlight python %}list = ['one', 'two']
list[1] = 'one'
print list
['one', 'one']{% endhighlight %}

As in from JS, if you assign one list to another, such as in the following

{% highlight python %}reptiles = ['croc', 'gator']
animals = reptiles
animals.append('poodle', 'schnoodle')
{% endhighlight %}

then.. 
{% highlight python %}
print reptiles
> ['croc', 'gator','poodle', 'schnoodle']
#when the intended was ['croc', 'gator']
{% endhighlight %}

This is because assigning animals to reptiles will make it so that both lists have the same object reference. To avoid this.
{% highlight python %}animals = reptiles[:]{% endhighlight %}


