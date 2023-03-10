# Compiling from Rust to WebAssembly

Building our WebAssembly package

```bash
cargo install wasm-pack

wasm-pack build --target web
```

Serve the root directory of the project with a local web server

- Using Python:
`python3 -m http.server`
- Using VSCode extension:
`vscode-preview-server`

Load index.html from the web server:

- if you used the Python3 example: `http://localhost:8000`.
- if you used VSCode extension example: `http://localhost:8080/hello-wasm/index.html`.

An alert box appears on the screen, with Hello, WebAssembly! in it. We've successfully called from JavaScript into Rust, and from Rust into JavaScript.
