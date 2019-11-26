# Substrate Runtime-Contract Sample

A sample Substrate runtime showing interaction between runtime modules (pallets) and smart contracts (ink!).

## Custom types for Polkadot JS

```json
{
  "Foo": {
    "id": "u32",
    "data": "Vec<u8>"
  }
}
```

## Build

Install Rust:

```bash
curl https://sh.rustup.rs -sSf | sh
```

Initialize your Wasm Build environment:

```bash
./scripts/init.sh
```

Build Wasm and native code:

```bash
cargo build --release
```

## Run

Start a development chain with:

```bash
./target/release/node-template --dev
```

Detailed logs may be shown by running the node with the following environment variables set: `RUST_LOG=debug RUST_BACKTRACE=1 cargo run -- --dev`.

Additional CLI usage options are available and may be shown by running `cargo run -- --help`.