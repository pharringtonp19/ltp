- [The truth](https://www.tweag.io/blog/2020-04-16-exceptions-in-haskell/#fnref-2) of the matter is that throwing exceptions was never a problem for purity: the problem was catching exceptions
- [Whenever](https://www.tweag.io/blog/2020-04-16-exceptions-in-haskell/#fnref-2) a function has a precondition which cannot be checked by the type checker, violating it would ideally throw an imprecise exception
- Exceptions are kinda a little bit magic because they have semantics which can only be explained by the actual call stack.
