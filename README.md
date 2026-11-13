# Firefly Index Data

Verified-only Quark index packages published by firefly-indexer.

## Walnuts index

The Android client checks these sources in order:

1. GitHub Release

   ```text
   https://github.com/Tart7/firefly-index-data/releases/download/walnuts-latest/walnuts-manifest.json
   ```

2. jsDelivr Fastly

   ```text
   https://fastly.jsdelivr.net/gh/Tart7/firefly-index-data@main/walnuts/latest/walnuts-manifest.json
   ```

3. jsDelivr CDN

   ```text
   https://cdn.jsdelivr.net/gh/Tart7/firefly-index-data@main/walnuts/latest/walnuts-manifest.json
   ```

Each source contains the same `walnuts-manifest.json`,
`walnuts-index.db.gz`, and `SHA256SUMS`. The client verifies the
decompressed SQLite SHA256 before replacing the local index.
