## usage

See: https://github.com/WebAssembly/gc/interpreter

```sh
$ docker build . -t wasmgc

# convert wat to wasm
$ docker run -i -v "$PWD":/data wasmgc wasm -d /data/test.wat -o /data/test.wasm

# interpret wasm
$ docker run -i -v "$PWD":/data wasmgc wasm /data/test.wasm
```
