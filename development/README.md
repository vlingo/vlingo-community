# Development guidelines

:warning: __Work in progress__ :warning:

## Definition of Done

- The issue should describe briefly the feature. It should help others know that it aims to accomplish and which it's the feature scope
- Implementation follows the code style guidelines
- Implementation has the proper testing. Unit tests are usually enough, but some cases might require integration tests.
- [Documentation](../documentation/README.md)
  - If it exposes an API for third party → [docs.vlingo.io][docs]
  - If it's internal, a brief usage explanation on the same repository under `/docs` folder
  - Desired to have `javadocs` since they are published automatically to [javadoc.io/doc/io.vlingo/vlingo-actors][javadocs]

## Code style

### General

- Use __meaningful names__

### Visibility of Variables and Methods

- __public__ is used for any method that must have scope to any client code that lives in different packages. This is true of Action::Action(...) because dependent applications must be able to access this constructor from any proprietary (customer/client) package.

- __protected__ is used only for extending subclass of a given superclass. Currently in Action we don't allow extension, so there are no protected methods.

- __package (default)__ is highly necessary for libraries, allowing access to behaviors and state that may be gained only by other library components located in the same package. Various top-level vlingo-platform components use this because they are ultimately libraries and require "secret" access to internal behaviors and data.

- __private__ is used when no other component outside the declaring class may access a method or data, not even extending subclasses or package-related classes.

### Variables declaration

- Prefer __Immutability__. Use `final` always unless you do need make mutable state for a good reason.

### Copyright

Add the next copyright text on top of each Source File.

```
// Copyright © 2012-2018 Vaughn Vernon. All rights reserved.
//
// This Source Code Form is subject to the terms of the
// Mozilla Public License, v. 2.0. If a copy of the MPL
// was not distributed with this file, You can obtain
// one at https://mozilla.org/MPL/2.0/.
```

Configure your IDE to autoinclude the copyright

- [Configure copyright on Intellij IDEA](https://www.jetbrains.com/help/idea/copyright.html)

[docs]: https://docs.vlingo.io
[javadocs]: https://javadoc.io/doc/io.vlingo/vlingo-actors