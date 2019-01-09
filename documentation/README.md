# Documentation guidelines

:warning: __Work in progress__ :warning:

:warning: Some of the next points might not be applied yet, we're adopting it.

> Making the boring part less tedious.

Do a minimum of documentation is healthy for the project, for the author and the contributors.

The goal is help newcomers to have smooth onboarding on vlingo, so, we choose the documentation tool that help us reach that goal as faster as possible.

## Source code examples

The best way to share how a new feature works is code some use case. All features should have a source code example.

[github.com/vlingo/vlingo-examples][examples]

## Public documentation - [docs.vlingo.io][docs]

:busts_in_silhouette: When the feature is enough important, the component responsible will ask you for a sort of more _serious_ documentation. You will hav to coordinate with him/her.

Write access to docs.vlingo.io is limited.

## Component documentation - [JavaDocs][javadocs]

Add useful comments into __exposed API methods__.

Documenting the internal methods is a nice to have, and more if the method is doing some complex stuff that might not be easy to understand, but we won't ask you to document everything.

## Internal component documentation

Important architectural decisions should be documented under `/docs` folder on each component repository.

## Changelog

Keep track of changes on `CHANGELOG.md` file on each component repository.

## External material

In case you prefer to make a tutorial, guideline or sample code in your own Blog, Medium, GitHub or a Video, we will link your work to help others reach your learning material.

We keep the decision of listing or not.

[docs]: https://docs.vlingo.io
[examples]: https://github.com/vlingo/vlingo-examples
[javadocs]: https://javadoc.io/doc/io.vlingo/vlingo-actors