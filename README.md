This is the fork used by [Edita](//edita.vercel.app). The main changes are:

- Fixes for using Wasm binaries in Electron

- Static linking for languages that use extra libraries in custom scanners, which otherwise fail with Wasm errors when loaded dynamically.

To enable static linking, configure the paths in scripts/build-wasm and pass the `--static` option when building. See https://github.com/tree-sitter/tree-sitter/issues/949 for more details.
