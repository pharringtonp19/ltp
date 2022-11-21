# ltp
Learning to Program

> [families](https://www.cse.chalmers.se/~peterd/papers/DependentTypesAtWork.pdf) of types indexed by other types, not families of types indexed by elements of another type

- [ ] [YouTube Channel](https://www.youtube.com/watch?v=1vXdNNSmvJw&list=PLE-CSy3N6yEeYY5tx1u5IP3d_2xZOmpKO)
- [ ] [Adga for Math Lectures](https://www.mathstat.dal.ca/~selinger/agda-lectures/)
- [ ] [Textbook](https://plfa.github.io/20.07/Naturals/)
- [ ] [Reeds YouTube Channel](https://www.youtube.com/channel/UC8sjG717gknTmWIeTyGmUHw/videos)

- agda doesn't need type declarations
- [In](http://learnyouanagda.liamoc.net/pages/introduction.html#fnref1) Agda, the distinction between types and values does not exist. Instead, the language you use to manipulate type terms is exactly the same language that you use to manipulate values.

### Haskell
- [A](https://serokell.io/blog/haskell-typeclasses) typeclass defines a set of methods that is shared across multiple types.
- [A](https://serokell.io/blog/haskell-typeclasses) type has an instance of a typeclass if it implements the methods of that typeclass.
- [Functors](https://mmhaskell.com/monads/functors) are an abstract mathematical structure that we represent in Haskell with a typeclass, and this structure has particular "laws" associated with it that dictate its expected behavior. Monads are the same way!
- [In](https://stackoverflow.com/questions/7103864/what-are-practical-uses-of-applicative-style) practice, I mostly find myself using applicatives much in the same way like I use point-free style: To avoid naming intermediate values when an operation is more clearly expressed as a composition of other operations

### Lambda Calculus
- [Sellinger's Notes](https://arxiv.org/pdf/0804.3434.pdf)

### Algebraic Effects & Handlers
- [Ocaml](https://github.com/ocamllabs/ocaml-effects-tutorial), [YouTube](https://www.youtube.com/watch?v=plFFZcqBOyk)
- [This](https://overreacted.io/algebraic-effects-for-the-rest-of-us/) is the part you can’t do with try / catch. It lets us jump back to where we performed the effect, and pass something back to it from the handler
