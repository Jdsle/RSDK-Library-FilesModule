## RSDK-Library Files Module
###### Note - If you're looking for the website file manager UI, [that can be found here.](https://github.com/Jdsle/RSDK/blob/main/app/controls/files.tsx)
This compiles an empty Files.c - this will allow us to load the .wasm module, and access emscripten's file system, via the RSDK-Library file manager

### Building
```
emcmake cmake -B build
cmake --build build
```
