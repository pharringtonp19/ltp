# Learning to Program

`data Vec (X : Set) : N -> Set where`

> [So, when will an I/O action be performed?](http://learnyouahaskell.com/input-and-output#hello-world)

[Sellinger's Notes](https://arxiv.org/pdf/0804.3434.pdf) | Types and Programming Languages | Essentials of Programming Languages | Programming Language Pragmatics | Milner’s
pi-calculus book |  Hoare Logic and axiomatic semantics (e.g. Winskel, 1993)

> [The](https://www.schoolofhaskell.com/user/school/starting-with-haskell/basics-of-haskell/3-pure-functions-laziness-io) way the actions are glued together is the essence of the Monad. Since the glueing happens between the lines, the Monad is sometimes described as an "overloading of the semicolon." Different monads overload it differently.

### Intensional vs Extensional
- [In Intensional](https://youtu.be/bNG53SA4n48?list=PLQRKUSOIMEh1Arz0-WBgD_Pol4S50HATv&t=877) type theory all operations are extensional

### Type Theory
> [Types come first](https://youtu.be/bNG53SA4n48?list=PLQRKUSOIMEh1Arz0-WBgD_Pol4S50HATv&t=267)
> [Extensional Operations](https://youtu.be/bNG53SA4n48?list=PLQRKUSOIMEh1Arz0-WBgD_Pol4S50HATv&t=792) preserve isomorphisms

> [... Exihibits ad hoc polymorphism](https://youtu.be/2EdQFCP5mZ8?t=305)

> computational context.

- [Conor Hoekstra](https://twitter.com/code_report)
- [Ben Deane](https://www.youtube.com/watch?v=on7v8nlyaAg)

> [families](https://www.cse.chalmers.se/~peterd/papers/DependentTypesAtWork.pdf) of types indexed by other types, not families of types indexed by elements of another type

- [ ] [YouTube Channel](https://www.youtube.com/watch?v=1vXdNNSmvJw&list=PLE-CSy3N6yEeYY5tx1u5IP3d_2xZOmpKO)
- [ ] [Adga for Math Lectures](https://www.mathstat.dal.ca/~selinger/agda-lectures/)
- [ ] [Textbook](https://plfa.github.io/20.07/Naturals/)
- [ ] [Reeds YouTube Channel](https://www.youtube.com/channel/UC8sjG717gknTmWIeTyGmUHw/videos)

- agda doesn't need type declarations
- [In](http://learnyouanagda.liamoc.net/pages/introduction.html#fnref1) Agda, the distinction between types and values does not exist. Instead, the language you use to manipulate type terms is exactly the same language that you use to manipulate values.

### Haskell

- Concrete Types `->` Type Constructors

- `wrap it with a newtype`

##### Actions
  - [Actions](https://www.haskell.org/tutorial/io.html) are defined rather than invoked within the expression language of Haskell. Evaluating the definition of an action doesn't actually cause the action to happen. Rather, the invocation of actions takes place outside of the expression evaluation we have considered up to this point.
  - [Produce](https://book.realworldhaskell.org/read/io.html#ftn.id610368) an effect when performed, but not when evaluated. That is, they only produce an effect when called by something else in an I/O context
  
- [Bartoz](https://www.schoolofhaskell.com/school/starting-with-haskell/basics-of-haskell/function-application)
- [Exceptions](https://markkarpov.com/tutorial/exceptions.html#the-motivation-for-exceptions)
- Continuations
- Comma Category
- [Detailed Examples](https://devtut.github.io/haskell/foldable.html#flattening-a-foldable-structure-into-a-list)
- [A](https://serokell.io/blog/haskell-typeclasses) typeclass defines a set of methods that is shared across multiple types.
- [A](https://serokell.io/blog/haskell-typeclasses) type has an instance of a typeclass if it implements the methods of that typeclass.
- [Functors](https://mmhaskell.com/monads/functors) are an abstract mathematical structure that we represent in Haskell with a typeclass, and this structure has particular "laws" associated with it that dictate its expected behavior. Monads are the same way!
- [In](https://stackoverflow.com/questions/7103864/what-are-practical-uses-of-applicative-style) practice, I mostly find myself using applicatives much in the same way like I use point-free style: To avoid naming intermediate values when an operation is more clearly expressed as a composition of other operations

  

### Algebraic Effects & Handlers
- [Ocaml](https://github.com/ocamllabs/ocaml-effects-tutorial), [YouTube](https://www.youtube.com/watch?v=plFFZcqBOyk)
- [This](https://overreacted.io/algebraic-effects-for-the-rest-of-us/) is the part you can’t do with try / catch. It lets us jump back to where we performed the effect, and pass something back to it from the handler
- [Effect Handlers](https://youtu.be/VEhkhxoGJSk?t=318): 
   - A mechanism for programming with user-defined effects. Modular basis for non-local control-flow mechanisms
   - First-Class restartable exceptions 

### Combinators
- Patterns of composition

### CC Plus Plus
- [Course Notes](https://ocw.mit.edu/courses/6-096-introduction-to-c-january-iap-2011/resources/mit6_096iap11_lec02/)

### Interpreters
- [Meetup](https://www.meetup.com/programming-languages-toronto-meetup/events/289784058/)
- [Textbook](http://www.craftinginterpreters.com/a-map-of-the-territory.html)
