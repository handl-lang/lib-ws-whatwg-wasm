# lib-ws-whatwg-wasm

WHATWG WebSocket surface for wasm/JS hosts.

Part of the `handl-lang` org split (ADR-0128). History is a `git subtree
split` of the platform monorepo's `ws_whatwg_wasm/` (via `web`).

## Layout

```text
src/        the .hnl sources
pkg.hnl     dependencies, when any: `{ deps: { <name>: "branch:<ref>" } }`
```

## Gate

```bash
HNL=../host-cli/target/debug/hnl scripts/hnl-gate.sh
```
