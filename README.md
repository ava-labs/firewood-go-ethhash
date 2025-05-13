# firewood-go

firewood-go provides a Golang FFI wrapper for [Firewood](https://github.com/ava-labs/firewood/).

This repo serves serves as a mirror, maintained by Firewood CI, to include both the Firewood Golang FFI source code and attach pre-built binaries directly to source. This enables the Go toolchain to import Firewood and use the pre-built binaries with CGO without worrying about the fact it's implemented in Rust.

For complete documentation, see [Firewood FFI](https://github.com/ava-labs/firewood/tree/main/ffi)
