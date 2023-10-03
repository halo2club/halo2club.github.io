# 2. proof system modifications
the original `zcash/halo2` consists of:
- an **optimising system** compatible with UltraPlonK arithmetisation;
- the UltraPlonK **interactive oracle proof**; and
- the inner product argument, used as a **polynomial commitment scheme**.

popular forks of `halo2` have incorporated proof system modifications across the stack.
## arithmetisation
- Axiom’s [`halo2-base`](https://github.com/axiom-crypto/halo2-lib/tree/community-edition/halo2-base), a frontend to halo2’s cell assignment API

## interactive oracle proof (IOP)
- `privacy-scaling-exploration`’s [`Challenge` API](https://github.com/privacy-scaling-explorations/halo2/blob/0c3e3b569519b86653a64f412bbce17e4e8acac4/halo2_proofs/src/plonk/circuit.rs#L586-L591), which introduces multiple phases to the IOP

### lookups
- [`mvlookup`](https://github.com/geometryresearch/halo2/tree/pse-mvlookup): implementation of log-derivative based [MVLookup](https://github.com/Orbis-Tertius/MVlookups/blob/main/MVlookup.pdf)
- [`cq`](https://github.com/geometryresearch/halo2-cq/tree/halo2-cq): implementation of cached quotients lookup [`cq`](https://eprint.iacr.org/2022/1763)

## commitment scheme
- `privacy-scaling-exploration`’s [integration of the KZG](https://github.com/privacy-scaling-explorations/halo2/tree/main/halo2_proofs/src/poly/kzg) polynomial commitment scheme

## general experimentation
- [`han0110/plonkish`](https://github.com/han0110/plonkish): implementations of HyperPlonK, Sangria, ProtoStar, and more