---
layout: home
title: A collection of Julia anti-patterns
---

Learning what to do in Julia by learning what not to do in Julia.

[Julia](https://julialang.org) is a modern, powerful programming language growing in popularity. Like any language it has unique and appealing features, but also pitfalls and gotchas. Users coming from higher-level languages such as Python or R may in particular struggle and fall for one of these errors.

This collection of worst practices will hopefully act as a reference and give you some of the tools you need to write lightning fast, error-free, maintainable Julia code. Parts are heavily influenced by the Julia manual - particularly the [Performance Tips](https://docs.julialang.org/en/stable/manual/performance-tips), [Style Guide](https://docs.julialang.org/en/stable/manual/style-guide) and [Noteworthy Differences](https://docs.julialang.org/en/stable/manual/noteworthy-differences) sections of the manual - but take a slightly more informal and opinionated tone. This whole site was influenced by [The Little Book of Python Anti-Patterns](https://docs.quantifiedcode.com/python-anti-patterns/index.html).

## Sections

- [Correctness]({{ site.baseurl }}{% link pages/correctness.md %})
- [Performance]({{ site.baseurl }}{% link pages/performance.md %})
- [Maintainability]({{ site.baseurl }}{% link pages/maintainability.md %})
- [Packaging]({{ site.baseurl }}{% link pages/packaging.md %})
- [Community]({{ site.baseurl }}{% link pages/community.md %})
- [Switching from Python]({{ site.baseurl }}{% link pages/switching_from_python.md %})
- [Switching from R]({{ site.baseurl }}{% link pages/switching_from_r.md %})
- [Switching from Matlab]({{ site.baseurl }}{% link pages/switching_from_matlab.md %})

## Contributing

Please contribute further worst practices, or refine existing wording, via [GitHub](https://github.com/jgreener64/julia-anti-patterns).
