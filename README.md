> **Renty fork — branch `renty/placement-transitions`.** This branch is upstream
> `v0.27.1` plus one change (two commits): MapLibre's placement transitions can be switched
> off and on (`MapLibreMap.placementTransitionsEnabled`,
> `MapLibreMapController.setPlacementTransitionsEnabled`), applied again on every
> style load, and switching them repaints the map. With them on, MapLibre places
> symbols at most every 300 ms, so a symbol whose data just changed can be drawn,
> hidden and faded back in. Renty switches them off around its own data updates.
> Android and iOS; ignored on web.
>
> **Upgrading:** rebase this branch's commits onto the new upstream tag, push it as
> `renty/placement-transitions-<version>`, and pin the new commit SHA in Renty's
> `renty_app/pubspec.yaml`. No upstream pull request is planned.

maplibre_gl/README.md