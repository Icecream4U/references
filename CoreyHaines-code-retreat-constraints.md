## Example constraints

#### Lines of code per method <= 3
We all have seen methods we consider too large. But what size is reasonable for a method? Let’s go to the extreme and say three lines is the maximum.

#### No in-method branching statements
Branching statements, such as the notorious if, are a form of procedural polymorphism. Let’s work on improving our object skills by finding other mechanisms to get the same effect. Prefer type-based polymorphism or lookup tables.

#### No primitives across method boundaries (input or output)
The only types that can be passed across method boundaries (inputs and outputs) are ones that we have defined. No data primitives, such as booleans, integers or strings. You also are not allowed to use primitive data structures such as Lists, Arrays or Enumerables. Focus instead on understanding what the types represent and building types for those concepts.

#### Mute ping-pong pairing
One member of the pair writes the unit tests, the other member writes the code to turn those tests green. You can think of the roles as “test redder” and “test greener.” This is standard. However, the only communication allowed between partners is through the tests and the code. And no cheating by putting a bunch of comments!

#### Find the loophole
Generally coupled with ping-pong pairing, one pair writes the tests, the other pair tries to get those tests passing. The catch is that the pair working to get the tests passing writes the wrong code. How long can you go before the tests force you into a “correct” algorithm. Here’s the catch, though: you must write production-level code, think of it as code you would show a prospective employer.

#### No return values
Similar to the principle of “tell, don’t ask” this constraint takes away your ability to return values from a function. Focus entirely on sending messages to objects.

#### Program like it’s 1969
Compilation is expensive and not real-time. You can only run your code twice during the session: first at the 30-minute mark, the second at the 44-minute mark. Better pay attention to syntax!

#### Object Calisthenics
Practicing different aspects of object-oriented design is great, but what happens when you put everything together in an extreme situation? Object Calisthenics provides a set of rules that really work out your OO understanding.
