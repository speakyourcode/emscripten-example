# Emscripten Tutorial example

This example is taken from the
[Tutorial](https://emscripten.org/docs/getting_started/Tutorial.html#generating-html).
The files have been generated with:

```
emcc src/hello_world.c -o html/helloWorld.js -s ENVIRONMENT="web" -s EXPORTED_FUNCTIONS='["_malloc", "_free", "_hello"]' -s MODULARIZE=1
```

Emscripten versions:

```
emcc (Emscripten gcc/clang-like replacement + linker emulating GNU ld) 3.1.32 (eab98adf462c39f3c31d348331c4830bcaa36949)
```

## Server

To run the server:

```
npx http-server -p 5514 html
```
