# Upstream

This repository is the Mindaeon-owned fork of [cloudflare/workers-sdk](https://github.com/cloudflare/workers-sdk) (MIT OR Apache-2.0).
Developer tooling for platform apps (task R5.3). Tracked at a release tag of the command-line tool; the line is its major version.

| | |
|---|---|
| Tracked line | `wrangler-4` |
| Last merged tag | `wrangler@4.146.0` |
| Last merged commit | `b4954c17b93a8da7223c7fa5b128a27812f18b86` (2026-10-01) |
| Recorded | 2026-10-03 |

## Branches

| Branch | Content |
|---|---|
| `upstream/wrangler-4` | An exact mirror of the upstream tag above. Never committed to by hand |
| `mindaeon/wrangler-4` | `upstream/wrangler-4` plus the patches listed in [PATCHES.md](PATCHES.md). The branch that is built from |

Builds are tagged `<upstream version>-m.<n>`. Our changes live in new files, or in an upstream file between
`mindaeon_change start` and `mindaeon_change end` comments that give the reason.

## Taking a new upstream version

1. Fetch the upstream tag and fast-forward `upstream/wrangler-4` to it.
2. Merge `upstream/wrangler-4` into `mindaeon/wrangler-4`; resolve patch by patch and drop a patch upstream now covers.
3. Run the licence check, the provenance gate, the security scan and the tests.
4. Update the table above and [PATCHES.md](PATCHES.md).
