# Note

This branch is just a work around to fix [a wasm bug](https://github.com/tomaka/wasm-timer/pull/13).

# Wasm-timer

Exports the `Instant`, `Delay`, `Interval` and `Timeout` structs.

On non-WASM targets, this re-exports the types from `tokio-timer`.
On WASM targets, this uses `web-sys` to implement their functionalities.
