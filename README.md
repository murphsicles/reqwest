# @net/reqwest — High-Level HTTP Client for Zeta

Auto-converted from [reqwest](https://crates.io/crates/reqwest) v0.13.3 via [Dark Factory](https://github.com/murphsicles/dark-factory).

## Features
- **JSON** — automatic serialization/deserialization via `@encoding/serde_json`
- **Multipart** — multipart form upload with streaming
- **TLS** — HTTPS support via native-tls or rustls
- **Cookies** — automatic cookie store and session management
- **Redirect** — configurable redirect following policy
- **Proxy** — HTTP and SOCKS5 proxy support
- **Streaming** — streaming request and response bodies
- **Timeouts** — connect, read, and write timeouts

## Usage
```zeta
let client = reqwest::Client::new();
let resp = client.get("https://api.example.com/data")
    .header("Authorization", "Bearer token")
    .send()
    .await?;
let body: serde_json::Value = resp.json().await?;
```

## Stats: ~8,909 lines across 40 source files, 0 unsupported items

## License
MIT