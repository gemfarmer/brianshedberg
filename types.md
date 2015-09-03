---
layout: page
permalink: /types/
---

JS Types: Number, String, Array, Object

# Numbers
In JS, all numbers belong to the Number type

In Python, things are a bit more sophisticated
* Integers
* Floats

# Type concatenation

Strings cannot be concatenated with integers or floats. Instead:

{% highlight python %}
print int('1') + 1
2
{% endhighlight %}

or

{% highlight python %}
float_concatenated = float('1.1') + 1
print float_concatenated
{% endhighlight %}

but the following is not allowable, because it tries to force rounding on a float...

{% highlight python %}
print int('1.1') + 1
{% endhighlight %}

In all of these cases, we are interpolating the value from one type to another before concatenating it with the other values.

# Strings

Strings have a method called .format() that will help with string interpolation.
For example

{% highlight python %}phrase = 'Chris has {0} arms, {1} head and {2} fingers'.format(num_arms, num_heads, num_fingers){% endhighlight %}

alternatively, the following would work, but would be more confusing

{% highlight python %}phrase = 'Chris has {1} arms, {2} head and {0} fingers'.format(num_fingers, num_arms, num_arms){% endhighlight %}

alternatively,

{% highlight python %}
print "{name} has {num_heads} heads and {num_arms} arms".format(
    name="Zaphod", num_heads=2, num_arms=3
) 
{% endhighlight %}

