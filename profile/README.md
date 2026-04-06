# `cmakefmt`

`cmakefmt` is a fast, workflow-first CMake formatter built in Rust.

It exists to replace the aging Python `cmake-format` tool with a single native
binary that is easy to install, fast enough for pre-commit and CI, and capable
enough for real project use.

## What You Will Find Here

- The main formatter repository: [`cmakefmt/cmakefmt`](https://github.com/cmakefmt/cmakefmt)
- Documentation: [cmakefmt.dev](https://cmakefmt.dev)
- Releases and install guidance: [latest releases](https://github.com/cmakefmt/cmakefmt/releases)
- Rust crate: [`cmakefmt-rust` on crates.io](https://crates.io/crates/cmakefmt-rust)

## Why `cmakefmt`?

- Fast enough for editor-on-save, pre-commit hooks, and CI
- Distributed as one native binary, with no Python environment to manage
- Designed around real workflows: `--check`, `--diff`, `--staged`, `--changed`,
  machine-readable reports, and config introspection
- Aware of custom command signatures, so project-specific macros and functions
  format sensibly
- Built to preserve comments, support formatter disable regions, and behave
  predictably across whole repositories

## Quick Start

```bash
brew install cmakefmt/cmakefmt/cmakefmt
cmakefmt --version
cmakefmt --check .
cmakefmt --in-place .
```

Rust users can also install via:

```bash
cargo install cmakefmt-rust
```

## Start Here

- [Getting Started](https://cmakefmt.dev/getting-started/)
- [CLI Reference](https://cmakefmt.dev/cli/)
- [Config Reference](https://cmakefmt.dev/config/)
- [Migration from `cmake-format`](https://cmakefmt.dev/migration/)
- [Performance](https://cmakefmt.dev/performance/)
- [Library API](https://cmakefmt.dev/api/)

## Status

`cmakefmt` is actively maintained and already usable on real projects. It is
still pre-`1.0`, so formatter behavior and packaging details may continue to
evolve as the tool matures.

## Contributing

Issues, bug reports, regression cases, and pull requests are welcome in
[`cmakefmt/cmakefmt`](https://github.com/cmakefmt/cmakefmt).
