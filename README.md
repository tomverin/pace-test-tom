# Pace Test (Phase 0)

Ephemeral test site for validating the terrain-aware adaptive pace model
designed for Corsica 555 race-day companion. Tested on a Crozet → Crêt
de la Neige loop (47 km / 1500 D+) before scaling to the full race site.

**Live**: https://tomverin.github.io/pace-test-tom/

Built from `scripts/race/build_pace_test_site.py` in the private
training-journal repo. Will be deleted after the model is validated.

Current V1 test scope:
- route-scoped storage keys
- GPS session cache and automatic opening fix
- new-session reset before a ride
- frequent refreshes accumulate to the latest eligible 5 min anchor
- loop and projection-jump guards for bad ratio updates
- stop segments excluded without losing the current position as next anchor
- POI modes: upcoming 30 km or all, with water/solid/services filters
- clickable POI list rows that center and open the map marker
