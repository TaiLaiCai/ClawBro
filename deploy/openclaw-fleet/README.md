# OpenClaw Fleet Deployment

This adds a working fleet deployment layout for multi-worker OpenClaw containers.

## Included

- `compose/docker-compose.yml` — 4 worker containers (`oc-a`..`oc-d`)
- `compose/entrypoint-worker.sh` — worker entrypoint adapted for fleet use

## Fixes included

- uses the image entrypoint flow instead of bypassing configuration generation
- preserves env-driven model selection (`OPENCLAW_PRIMARY_MODEL`)
- enables hooks configuration from env
- avoids interactive `openclaw doctor` during worker boot
- fixes nginx browser proxy to use the local browser control endpoint
- exposes worker HTTP entrypoint on port `8080` so container health checks pass normally

## Notes

This layout expects per-worker env/config/data directories under `/opt/openclaw-fleet/workers/<id>/...`.
