## Files Module
###### There's probably an easier way to do this, but...
This compiles an empty Files.c - this will allow us to load the .wasm module, and access emscripten's file system, via the RSDK-Library file manager

### Building
```
emcmake cmake -B build
cmake -B build
```
