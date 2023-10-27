# 1. developer tooling and libraries
*`halo2` has benefited from an incredible range of community-built developer tooling.*
## frontends and interfaces
- [halo2repl](https://halo2repl.dev): a web browser interface to write halo2 circuits with Javascript bindings for halo2-lib.

## domain-specific languages
- [Chiquito](https://github.com/privacy-scaling-explorations/chiquito): a high-level structured language for implementing zero knowledge proof applications that compiles to the `halo2` backend.
- [powdr](https://github.com/powdr-labs/powdr): an extended polynomial identity (PIL) and zk-focused assembly (zkASM) language written in Rust, focused on modularity and excellent developer experience. Supports `halo2` backend.
- [zkas](https://github.com/darkrenaissance/darkfi/tree/master/src/zkas) (DarkFi): a toolchain consisting of a lexer, parser, static and semantic analyzers, and a binary code compiler.

## libraries
- [`halo2wrong`](https://github.com/privacy-scaling-explorations/halo2wrong): applications involving non-native arithmetic
- [`halo2-lib`](https://github.com/axiom-crypto/halo2-lib): primitives for writing circuits, including
    - `halo2-base`: an API using a simple vertical gate;
    - `halo2-ecc`: elliptic curve cryptography primitives
- [`tachyon`](https://github.com/kroma-network/tachyon/tree/main/vendors/halo2) [WIP]: accelerated library using CUDA

## other primitives
- [`halo2-rsa`](https://github.com/zkemail/halo2-rsa) (zk-email): RSA verification circuit
- [`halo2-regex`](https://github.com/zkemail/halo2-regex) (zk-email): regex verification circuit
- [`halo2-base64`](https://github.com/zkemail/halo2-base64) (zk-email): base64 decoding circuit

## formal verification
- [Automated Analysis of Halo2 Circuits](https://eprint.iacr.org/2023/1051.pdf) [Soureshjani et al, 2023]: detecting under-constrained `halo2` circuits using an SMT solver.
    - implementation: [quantstamp/halo2-analyzer](https://github.com/quantstamp/halo2-analyzer)
