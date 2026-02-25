# tree-sitter-wasm-typescript-bindings
"TypeScript declarations (.d.ts) for Tree-sitter WebAssembly module compiled with Emscripten. Bindings automáticos para usar el parser en browser/Node.js"
# Tree-sitter WASM TypeScript Bindings

Declaraciones TypeScript para el módulo WebAssembly de **Tree-sitter** generado vía Emscripten.

## ¿Qué es?

Bindings de bajo nivel para interactuar con el core de Tree-sitter en WebAssembly.

**Nota:** Para la mayoría de los casos usa el paquete oficial [`web-tree-sitter`](https://www.npmjs.com/package/web-tree-sitter) que ya trae tipos más amigables.

## Instalación

```bash
npm install tu-usuario/tree-sitter-wasm-typescript-bindings

import MainModuleFactory from 'tree-sitter-wasm-typescript-bindings';

const module = await MainModuleFactory();
const parserPtr = module._ts_parser_new_wasm();
// ... etc
