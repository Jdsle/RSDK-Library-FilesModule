## RSDK-Library Files Module
###### Note - If you're looking for the website file manager UI, [that can be found here.](https://github.com/Jdsle/RSDK/tree/main/app/pages/files.tsx)
This compiles an empty Files.c - this will allow us to load the .wasm module, and access emscripten's file system, via the RSDK-Library file manager

...I was originally planning on having all engine source code here but decided that it would be better if they were their own repositories - so now, there's just this mostly empty repo, that compiles... a blank c file! awesome

### Building
```
emcmake cmake -B build
cmake -B build
```
