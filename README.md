# Archived / superseded

> **This repository is no longer developed.** FDTD Online now lives in the monorepo **[abc0990cba/node-addons-rust](https://github.com/abc0990cba/node-addons-rust)** (see [PR #1](https://github.com/abc0990cba/node-addons-rust/pull/1) and the monorepo README). Do not develop here — keep this tree as historical reference only.

---

## Legacy physics notes (historical)

kappa is used to "squeeze the wave", kappa=1 means the wave will propagate inside the PML without any "squeezing" effect. Kappa can be as large as to 10 but this is related to other parameters, such as power scaling, sigma and others. General sense is if kappa is too large, you have to scale kappa from 1 to kappa_max this will cause stiff jump between FDTD cells and will cause reflection, thus kappa=1 but no larger than 10 is in my personal preference, however, again I need to emphasize its related to your choices of other parameters.

As to alpha, it should be a small number, the true meaning of alpha is still on-going research in my personal point of view.
