# digipin

Rust implementation of the official DIGIPIN encoding and decoding algorithm.

## Usage


```toml
[dependencies]
digipin = { package = "digipin-rs", version = "0.1" }
```

```rust
use digipin::{encode, decode, Location};
let location = Location {     latitude: 28.622788,     longitude: 77.213033, };
let digipin = encode(location)?;
let decoded = decode(&digipin)?;
```
