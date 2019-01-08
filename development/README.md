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

[docs]: https://docs.vlingo.io
[javadocs]: https://javadoc.io/doc/io.vlingo/vlingo-actors