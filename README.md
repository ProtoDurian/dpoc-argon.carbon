# dpoc-argon.carbon

Platform repo for `argon` — the drill template platform (zinc). `platform.yaml` holds the platform facts
(landscapes/stages per PLAN §8, maturity). `infra/app` renders a ConfigMap
`argon-platform` into namespace `argon`; `infra/primordial` is empty-but-valid
(service repos own the dependency records).

TEMPLATE note (argon): not pushed until the drill creates it.

## Release
Push a tag `vX.Y.Z` (needs `DPOC_REG_PASSWORD`): pushes charts
`reg.dpoc.specpenguin.dev/charts/dpoc-argon:X.Y.Z` and `.../dpoc-argon-primordial:X.Y.Z` (no image).
