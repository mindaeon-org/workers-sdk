---
"@cloudflare/codemods": patch
---

Enable type generation by default in Wrangler configs created by `cf migrate`.

Previously, migrating a Wrangler config without `dev.generate_types` wrote `types.generate: false`, disabling development type generation. An explicit `dev.generate_types: false` still disables it.
