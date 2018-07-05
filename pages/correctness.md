---
layout: page
title: Correctness
---

## Over-specifying function arguments

Annotating function arguments with types can prevent the function being called with the wrong arguments, as well as making the intent of the function clear. However, contrary to some people's beliefs, it does not lead to improved performance because Julia compiles a new version of the function for each combination of input types. A common mistake is to over-specify the type of an argument when actually a less strict abstract type is more appropriate.

### Anti-pattern

{% highlight julia %}
myfunction(x::Int64, y::Int64) = 2*x + y
{% endhighlight %}

### Best practice

If you want the function to only work on integers, use the abstract container type `Integer`:

{% highlight julia %}
myfunction(x::Integer, y::Integer) = 2*x + y
{% endhighlight %}

However this function could work on any real number:

{% highlight julia %}
myfunction(x::Real, y::Real) = 2*x + y
{% endhighlight %}

In fact, it can work on any `x` and `y` where `*` and `+` are defined, so the following might also be appropriate:

{% highlight julia %}
myfunction(x, y) = 2*x + y
{% endhighlight %}
