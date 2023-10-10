# Projects
*`halo2` has been used in some weird and wonderful circuits, including: private transfers, proof of solvency, coprocessors, machine learning models, virtual machines, zk-email, Wordle, and more.*

> please note that many of the projects listed here are still under development and not to be used in production.

## virtual machines and execution environments
- [zkEVM](https://github.com/scroll-tech/zkevm-circuits) (Scroll): a validity proof for Ethereum transactions, powering the [Scroll succinct rollup](https://scroll.io/).
- [Taiga](https://github.com/anoma/taiga) (Anoma): a unified execution environment handling transparent, shielded, and private data access and operations.
- [zkWASM](https://github.com/DelphinusLab/zkWasm) (Delphinus Lab): the WASM virtual machine written in `halo2` circuits.
- [zkVM](https://github.com/darkrenaissance/darkfi/blob/master/src/zk/vm.rs) (DarkFi): a general-purpose zkSNARK virtual machine.

## machine learning
- [ezkl](https://github.com/zkonduit/ezkl) (ZKonduit): an engine for doing inference for deep learning models and other computational graphs in a zk-SNARK.
- [zkml](https://github.com/ddkang/zkml): a framework for constructing proofs of ML model execution in zk-SNARKs.

## coprocessors
- [Axiom coprocessor](https://github.com/axiom-crypto/axiom-eth): prove facts about Ethereum on-chain data via aggregate block header, account, and storage proofs.

## financial privacy
- [Zcash Orchard](https://github.com/zcash/orchard): private token transfers
- [Summa](https://github.com/summa-dev/summa-solvency): zk proof of solvency

## real-world protocols
- [Proof of Email](https://github.com/zkemail/#halo2-zk-email): prove facts about emails with the same trust assumption as the email domain.
    - demo projects: https://prove.email/
- [webauthn-halo2](https://github.com/zkwebauthn/webauthn-halo2): proving and verifying WebAuthn with `halo2`
- [eth-voice-recovery](https://github.com/SoraSuegami/voice_recovery_circuit)
## others
- [Zordle](https://github.com/nalinbhardwaj/zordle): zk Wordle
