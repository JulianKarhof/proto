# Shared Protocol Buffers

This repository contains protocol buffers which are shared across pog projects and can be used to interact with the different api's safely.

APIs are append only. Fields that aren't used anymore can only be updated for major new API versions or depricated and replaced. Old fields should first be marked as depricated and later commented out without their id being reused.

## Supported languages

### Rust

Currently prepackaged types are only provided for rust:

`cargo.toml`

```toml
[dependencies]
pog-proto = {git = "https://github.com/pognetwork/proto"}
```

Cargo pins dependencies, so after pushing a new change to this repo, be sure to run `$ cargo update` in the project depending on this. Also, remember to reload your IDE since the rust language server often doesn't pick up the changes in dependencies.

### Typescript

Typescript support will follow soon.
