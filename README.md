# osmos-transport

Peer-to-peer sync between your own devices, with no server in between.

> **Not started.** This repository holds the plan; the protocol comes first, then the code.

## The idea

Two devices that belong to the same person find each other, prove who they are, and exchange only what the other side is missing. The first user will be [Mythos](https://github.com/mythoside): keeping a manuscript in step between a desktop and a phone.

- **Transport:** QUIC (TLS 1.3), through [`quinn`](https://github.com/quinn-rs/quinn)
- **Discovery:** mDNS on the local network first
- **Identity:** a key pair per device
- **Data:** content-addressed with BLAKE3, so a device can ask for exactly what it lacks and verify what it gets

## License

MIT, see [LICENSE](./LICENSE).
