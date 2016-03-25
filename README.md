# catbird

[![Build status](https://img.shields.io/travis/travisbrown/catbird/master.svg)](http://travis-ci.org/travisbrown/catbird)
[![Coverage status](https://img.shields.io/codecov/c/github/travisbrown/catbird/master.svg)](https://codecov.io/github/travisbrown/catbird)
[![Maven Central](https://img.shields.io/maven-central/v/io.catbird/catbird-finagle_2.11.svg)](https://maven-badges.herokuapp.com/maven-central/io.catbird/catbird-finagle_2.11)


This project provides [cats](https://github.com/non/cats) type class instances (and other useful
cats-related stuff) for various [Twitter Open Source](https://twitter.com/twitteross) Scala
projects.

It currently includes the following:

* Type class instances for `Future`, `Var`, and `Try` (including `Monad` or `MonadError`, `Semigroup`, and equality)
* Category and profunctor instances for `Service`
* An injection from [Finagle](https://github.com/twitter/finagle) services to Kleisli arrows over
  `Future`
* A bijection from `Try[A]` to `Xor[Throwable, A]`

These are reasonably well-tested (thanks to [discipline](https://github.com/typelevel/discipline)).

## License

Licensed under the **[Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)** (the "License");
you may not use this software except in compliance with the License.

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
