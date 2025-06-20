# firewood-go-ethhash

firewood-go-ethhash provides a Golang FFI wrapper for [Firewood](https://github.com/ava-labs/firewood/).

This repo serves serves as a mirror, maintained by Firewood CI, to include both the Firewood Golang FFI source code and attach pre-built binaries directly to source. This enables the Go toolchain to import Firewood and use the pre-built binaries with CGO without worrying about the fact it's implemented in Rust.

These binaries provide an Ethereum-compatible hashing scheme, emulating that of `HashDB` and `PathDB`. For example usage, see the [Firewood hashing tests](https://github.com/ava-labs/firewood/tree/main/ffi/tests/eth/eth_compatibility_test.go).
	
Although Firewood supports a more efficient version of merkle hashing for general purpose use, this is disabled for these pre-built binaries.

For complete documentation, see [Firewood FFI](https://github.com/ava-labs/firewood/tree/main/ffi).
