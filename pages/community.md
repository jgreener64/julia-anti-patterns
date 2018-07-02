---
layout: page
title: Community
---

## Not quoting code in backticks on forums

When posting code snippets on forums such as Slack or Discourse, many people paste code directly without enclosing it in backticks. Enclosing code in backticks - a single `` ` `` for inline code `like_this` and ```` ``` ```` for a block of code as a paragraph - makes it more readable and can provide syntax highlighting. See more at [Discourse](https://discourse.julialang.org/t/psa-how-to-quote-code-with-backticks/7530).

### Anti-pattern

Can anybody help me with the following code? I'm not sure what do does or how to use f.

open("in_file.txt") do f
    for line in eachline(f)
        println(2.0 * float(line) + 3.0)
    end
end

### Best practice

Can anybody help me with the following code? I'm not sure what `do` does or how to use `f`.

{% highlight julia %}
open("in_file.txt") do f
    for line in eachline(f)
        println(2.0 * float(line) + 3.0)
    end
end
{% endhighlight %}
