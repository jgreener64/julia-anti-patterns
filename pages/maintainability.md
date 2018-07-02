---
layout: page
title: Maintainability
---

## Not indenting code

Just because you don't have to indent code blocks with whitespace, doesn't mean you shouldn't. Indenting blocks of code aids readability and makes the intent of the scoping clear.

### Anti-pattern

{% highlight julia %}
function myfunction()
if condition()
println("condition met")
end
end
{% endhighlight %}

### Best practice

As a general recommendation, indent blocks of code with 4 spaces.

{% highlight julia %}
function myfunction()
    if condition()
        println("condition met")
    end
end
{% endhighlight %}

The exception is `module` blocks which are usually not indented as they often correspond to whole files.
