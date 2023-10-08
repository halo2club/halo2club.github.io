# 3. interoperability and standardisation
*`halo2` is one of many zero-knowledge proof systems in production: our community is keen to support interoperability and standardisation efforts across proof systems.*
## proof composition
- FRI verifiers written in `halo2`:
    - [`maxgillett/halo2-fri-gadget`](https://github.com/maxgillett/halo2-fri-gadget)
    - [`DoHoonKim8/stark-verifier`](https://github.com/DoHoonKim8/stark-verifier)
- [`halo2` backend for Noir](https://github.com/Ethan-000/halo2_backend) [WIP]
- [`snark-verifier`](https://github.com/privacy-scaling-explorations/snark-verifier): aggregation circuit and EVM verifier generator for halo2-KZG proofs
- [`halo2-solidity-verifier`](https://github.com/privacy-scaling-explorations/halo2-solidity-verifier): Solidity verifier generator for `halo2` proof with KZG polynomial commitment scheme on BN254

## arithmetisation
- [plaf: Plonkish Arithmetization Format](https://github.com/Dhole/polyexen/blob/master/plaf.md): a standard format for plonkish circuits that can be reused in components that work with plonkish arithmetization. The current implementation supports the halo2 frontend.
- [High Assurance Specification of the `halo2` Protocol](https://moneroresearch.info/index.php?action=resource_RESOURCEVIEW_CORE&id=187&browserTabID=) [SB23]: an executable specification of `halo2`'s proving system, realised using `hacspec`.
    - implementation: [hacspec_halo2](https://hvassaa.github.io/hacspec_halo2/)
- [Arithmetization of Functional Program Execution via Interaction Nets in Halo 2](https://eprint.iacr.org/2022/1211) [Hart22]: a description of interaction nets and how to arithmetise them in `halo2` circuits.
- [Arithmetization of Σ₁¹ relations with polynomial bounds in Halo 2](https://eprint.iacr.org/2022/1105.pdf) [HT22]: a method for compiling Σ₁¹ formulas into `halo2` circuits.

## standardisation
- the [ZKProof Standards](https://zkproof.org/) effort is working to standardise one zero-knowledge proof system; do get in touch if you're interested in collaborating with one of their working groups.
