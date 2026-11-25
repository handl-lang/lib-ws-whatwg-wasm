# lib-ws-whatwg-wasm

WHATWG WebSocket surface for wasm/JS hosts. Pure `.hnl`.

## Layout

| path | role |
| --- | --- |
| `src/index.hnl` | the implementation |
| `docs/ws_whatwg_wasm.yml` | design notes |
| `pkg.hnl` | package manifest — `modules: ["ws_whatwg_wasm"]` |
| `scripts/hnl-gate.sh`, `ci.sh` | the gate / bupha entry |

## Contract

- WHATWG WebSocket surface for wasm/JS hosts; siblings:
  `lib-ws-whatwg-c` (libcurl/native) and `lib-ws-c`
  (`concurrent-epoll`).

## Verification

```bash
HNL=../host-cli/target/debug/hnl scripts/hnl-gate.sh
```

## License

MIT.

<!-- myco:agent-awareness -->

## Agent awareness

- Session start / any work discussion: run `myco status --prompt`
  before proposing next steps — know the board first.
- User describes new work → offer to capture it (`myco todo add`,
  `issue new`, `proposal new`). Don't wait to be asked.
- Picking up a task: `myco resume <ID>` is the briefing.
- Wrapping up: `myco handoff <ID>` anything resumable; keep statuses
  honest (claimed → in-progress → blocked/done).

<!-- /myco:agent-awareness -->
