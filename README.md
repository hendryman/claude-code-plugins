# hendryman-plugins

Manuel Hendry's Claude Code plugins marketplace.

## Install

```
/plugin marketplace add hendryman/claude-code-plugins
/plugin install worktree-flow
```

## Plugins

### worktree-flow

Parallel-feature development for solo macOS PHP/web devs: one git worktree + one Apache port per feature, previewable in the browser, torn down automatically on merge.

Canonical source: <https://github.com/hendryman/claude-code-worktree-flow>

See [`worktree-flow/README.md`](./worktree-flow/README.md) for full docs.

## Structure

This repository aggregates plugins via git submodules. Each plugin lives in its own canonical repo and is mounted as a subfolder here. The `.claude-plugin/marketplace.json` references each subfolder via `source: "./<name>/"`.

To clone the full marketplace including plugin source:

```
git clone --recursive https://github.com/hendryman/claude-code-plugins.git
```
