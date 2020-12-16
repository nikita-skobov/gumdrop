This repository is a fork from [murarth/gumdrop](https://github.com/murarth/gumdrop)

The only change is to add another trait called `OptionsCore`, and a proc macro for this trait. `OptionsCore` is a copy of the `Options` trait, but with several methods removed, and a few minor things changed in the proc macro. the changes are:

- OptionsCore does not have usage
- OptionsCore has no methods for printing usage/exiting
- OptionsCore does not treat unknown options as errors
- OptionsCore does not treat extra free positional arguments as errors
- OptionsCore does not implicitly treat "-h" or "--help" as a special variable
- OptionsCore does not use the first letter of a field as the short form


# `gumdrop`

Option parser with custom derive support

[Documentation](https://docs.rs/gumdrop/)

## Building

To include `gumdrop` in your project, add the following to your `Cargo.toml`:

```toml
[dependencies]
gumdrop = "0.8"
```

## License

`gumdrop` is distributed under the terms of both the MIT license and the
Apache License (Version 2.0).

See LICENSE-APACHE and LICENSE-MIT for details.
