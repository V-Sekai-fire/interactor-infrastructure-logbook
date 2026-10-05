# interactor-infrastructure-logbook

A logbook of measured results kept beside their retractions, and a doc gate that checks the workspace's documents against its manifest.

## What it is for

The logbook records what was measured, with enough of the apparatus to re-run it, and keeps a
retraction next to what it retracts. The gate is a mix application with one module per concern,
and every check ships a negative control that must fail on broken input. It reads the manifest
from the `repo` checkout above this one, and the claims only a remote can answer run before a
push rather than in CI.

## Run

```sh
cd misc/checks
mix check
```

## Licence

MIT; see `LICENSE`.
