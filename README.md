# InfluxDB Bosh Release

### Updating the Release
- Go to scripts/sync-submodule-config and change the `checkout <tag version>` to the version you want.
- Run `scripts/sync-submodule-config`
- Run `git add . -u` to add the new changes.
- Run make a commit
- Run `bosh create release`.
- Make sure it works by deploying.
- When finished, run `bosh create release --final`
