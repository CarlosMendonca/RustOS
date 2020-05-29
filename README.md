# RustOS

## Set up

* Start from a clean slate with `cargo clean`
* Install and set up Rust nightly. With ASDF, the version is set up locally by the `.tool-versions` file. Check the version with `rustc --version`
* Install cargo xbuild dependencies
  * GCC with, for example `apt-get install gcc`
  * rust-src with `rustup component add rust-src`
* Install the cargo xbuild cross compiler with `cargo install cargo-xbuild`
* Install cargo bootimage with `cargo install bootimage` and build dependencies
  * `rustup component add llvm-tools-preview`

## Build

```bash
cargo bootimage
```