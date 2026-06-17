# Composable boundaries
> Small pieces compound

Module boundaries tell us when to stop and ship.

A good boundary lets one piece become complete enough to trust, reuse, and build from. Each finished library becomes a tool for the next project. Each narrow utility removes repeated pain. Over time, small pieces become infrastructure.

Small is not enough. Pieces compound when their interfaces are clear. “This input gives you that output” is often all one should need to know. Interfaces are meant to be used, not crossed.

Separation of concerns prevents fast work from becoming a house of cards. The more independent the parts, the less information leaks between them, and the easier it is to reason locally. Good boundaries reduce required context.

Abstractions are necessary but dangerous. They should be earned by repeated structure, not introduced because the model found a pattern-shaped hole. Stay close to the data when possible. Question every complexity and every abstraction.

Pain points become narrow tools; narrow tools compose; composed tools become infrastructure. That is how [compound capability][compound-capability] becomes practical, and why boring interfaces serve [context discipline][context-discipline].

[compound-capability]: ../telos/compound-capability.md
[context-discipline]: context-discipline.md
