---
layout: page
title: Switching from Python
---

## Overuse of `try/catch`

Python follows the principle _better to ask for forgiveness than permission_, which in practice means using `try/except` blocks with type checking on the error. In Julia the preference is to avoid the error using an initial check.

### Anti-pattern

Overuse of constructs such as:

{% highlight julia %}
try
    myfunction()
catch e
    if isa(e, DomainError)
        response()
    else
        rethrow()
    end
end
{% endhighlight %}

Though the above is far preferable to the below, which risks triggering a desired response for the wrong error.

{% highlight julia %}
try
    myfunction()
catch
    response()
end
{% endhighlight %}

### Best practice

{% highlight julia %}
if condition()
    myfunction()
else
    response()
end
{% endhighlight %}
