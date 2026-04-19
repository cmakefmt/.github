# `cmakefmt`

`cmakefmt` is a fast, correct CMake formatter built in Rust.

It replaces the aging Python `cmake-format` tool with a single native
binary that is easy to install, fast enough for pre-commit and CI, and
capable enough for real project use.

## Repositories

| Repository | Description |
|---|---|
| [`cmakefmt/cmakefmt`](https://github.com/cmakefmt/cmakefmt) | Main formatter — CLI, LSP server, library |
| [`cmakefmt/vscode-cmakefmt`](https://github.com/cmakefmt/vscode-cmakefmt) | VS Code extension |
| [`cmakefmt/cmakefmt-action`](https://github.com/cmakefmt/cmakefmt-action) | GitHub Action |
| [`cmakefmt/homebrew-cmakefmt`](https://github.com/cmakefmt/homebrew-cmakefmt) | Homebrew tap |

## Install

```bash
brew install cmakefmt/cmakefmt/cmakefmt   # macOS
pip install cmakefmt                      # any platform with Python
cargo install cmakefmt-rust               # any platform
conda install -c conda-forge cmakefmt     # conda-forge
```

Or download a pre-built binary from [GitHub Releases](https://github.com/cmakefmt/cmakefmt/releases/latest).

Also available on [winget](https://github.com/microsoft/winget-pkgs), the
[VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=cmakefmt.vscode-cmakefmt),
[Open VSX Registry](https://open-vsx.org/extension/cmakefmt/vscode-cmakefmt),
and as a [Docker image](https://ghcr.io/cmakefmt/cmakefmt).

## Why `cmakefmt`?

- **Fast** — 25× faster than `cmake-format`; fast enough for editor-on-save, pre-commit hooks, and CI
- **One binary** — no Python environment to manage
- **LSP server** — `cmakefmt lsp` provides format-on-save in any editor
- **Workflow-first** — `--check`, `--diff`, `--staged`, `--changed`, machine-readable reports, and config introspection
- **Custom command aware** — project-specific macros and functions format sensibly
- **Comments preserved** — barrier regions, fence blocks, and pragma support

## Quick Start

```bash
cmakefmt config init               # generate a starter .cmakefmt.yaml
cmakefmt .                         # preview formatted output
cmakefmt --diff .                  # view a unified diff of what would change
cmakefmt --in-place .              # apply formatting across the whole project
cmakefmt --staged --check          # use in pre-commit hooks
cmakefmt --path-regex 'src/.*' .   # format CMake files only under src/
```

## Documentation

- [Getting Started](https://cmakefmt.dev/getting-started/)
- [CLI Reference](https://cmakefmt.dev/cli/)
- [Config Reference](https://cmakefmt.dev/config/)
- [Editor Integration](https://cmakefmt.dev/editors/)
- [Migration from `cmake-format`](https://cmakefmt.dev/migration/)
- [Performance](https://cmakefmt.dev/performance/)
- [Playground](https://cmakefmt.dev/playground/)

## Contributing

Issues, bug reports, and pull requests are welcome in
[`cmakefmt/cmakefmt`](https://github.com/cmakefmt/cmakefmt).
