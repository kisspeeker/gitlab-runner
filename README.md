# GitLab Runner

## Bootstrap

1. Create GitLab **Group Runner**:
   - Tag: `self-hosted`
   - Run untagged jobs: enabled
   - Protected: enabled

2. Add `glrt-` token as `GITLAB_RUNNER_TOKEN` to `secrets.production.sops.env`.

3. Start local runner:
   ```bash
   mise install
   mise run build
   ```
