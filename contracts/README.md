
สำหรับ compiler rust🦀🦀 ให้เป็น wasm
cargo wasm
cargo schema

[alias]
wasm = "build --release --target wasm32-unknown-unknown"
wasm-debug = "build --target wasm32-unknown-unknown"
unit-test = "test --lib"
integration-test = "test --test integration"
schema = "run --example schema"


