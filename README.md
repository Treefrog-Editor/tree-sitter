This fork has the following changes for [Edita](//edita.vercel.app):

- fix environment detection in lib/binding_web/binding.js

- statically link langs that use libraries that aren't in exports.json (see https://github.com/tree-sitter/tree-sitter/issues/949), and update `Language.load` to get them from the main module, as emscripten requests the wasm files and merges them into the main module on startup

See https://gitlab.com/gushogg-blake/edita-release/-/blob/main/howto/tree-sitter.md for more details.
