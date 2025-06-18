# firewood-go-ethhash

firewood-go-ethhash provides a Golang FFI wrapper for [Firewood](https://github.com/ava-labs/firewood/).

This repo serves serves as a mirror, maintained by Firewood CI, to include both the Firewood Golang FFI source code and attach pre-built binaries directly to source. This enables the Go toolchain to import Firewood and use the pre-built binaries with CGO without worrying about the fact it's implemented in Rust.

These binaries provide an Ethereum-compatible hashing scheme, emulating that of `HashDB` and `PathDB` (see the [hashing tests](https://github.com/ava-labs/firewood/tree/main/ffi/tests/eth/eth_compatibility_test.go) for example usage). Although Firewood supports a more efficient version of  Merkle hashing for general purpose use, this is not available on these pre-built binaries, but may be provided in the future.

For complete documentation, see [Firewood FFI](https://github.com/ava-labs/firewood/tree/main/ffi).
