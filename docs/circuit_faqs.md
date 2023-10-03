# circuit FAQs
these questions and answers are mostly taken from the [`halo2` ecosystem Discord](https://discord.gg/NxUHAw8rGu); they are meant for circuit writers, not complete beginners. if some of these terms seem completely strange to you, the [halo2 book](https://github.com/zcash/halo2) is a good place to look them up.

#### do unassigned cells default to zero?
yes, unassigned cells are initialised to zero in the current implementation; but this is an arbitrary implementation choice, and we shouldn't rely on it being true. e.g. there was some discussion about randomising unassigned cells: https://github.com/zcash/halo2/issues/614

#### how do we decide which columns to reuse across chips?
currently, the reuse of advice columns is a manual decision, as the FloorPlanner has no way to horizontally optimise. this capability is intended to be introduced: see [zcash/halo2#195](https://github.com/zcash/halo2/issues/195).

#### does `halo2` support runtime configuration of circuits?
this is a feature we want to enable and are discussing in [zcash/halo2#550](https://github.com/zcash/halo2/issues/550). this is already supported in the `privacy-scaling-explorations/halo2` fork as a [feature flag](https://github.com/privacy-scaling-explorations/halo2/pull/168/files).

#### given a circuit object, can we estimate the minimum number of rows it will use?
this is currently not supported, and would likely involve writing a `FloorPlanner` that only returns the number of rows used.