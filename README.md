Serde support for Hyper types
=============================

This crate provides wrappers and convenience functions to support [Serde] for
some types defined in [cookie], [Hyper], [hyperx], [mime] and [time].

[cookie]: https://github.com/alexcrichton/cookie-rs
[Hyper]: https://github.com/hyperium/hyper
[hyperx]: https://github.com/dekellum/hyperx
[mime]: https://github.com/hyperium/mime.rs
[Serde]: https://github.com/serde-rs/serde
[time]: https://github.com/rust-lang-deprecated/time

The supported types are:

* `cookie::Cookie`
* `hyperx::header::ContentType`
* `hyperx::header::Headers`
* `hyper::Method`
* `hyper::Uri`
* `mime::Mime`
* `time::Tm`

What is `hyperx`? As of hyper 0.12, the `header` module was removed and replaced
with the `http` types like `HeaderMap`. All typed headers like `ContentType` were
removed [for now](https://github.com/hyperium/hyper/blob/master/CHANGELOG.md).

`hyperx` is a fork that contains all the headers that were removed as well as
a conversion from `Headers` to the new `HeaderMap` type.

For more details, see the crate documentation.

## License

hyper_serde is licensed under either of

 * Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or
   http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license ([LICENSE-MIT](LICENSE-MIT) or
   http://opensource.org/licenses/MIT)

at your option.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in hyper_serde by you, as defined in the Apache-2.0 license,
shall be dual licensed as above, without any additional terms or conditions.
