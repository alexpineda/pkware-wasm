# pkware-wasm
[StormLib](https://github.com/ladislav-zezula/StormLib) Implode and Explode algorithms for javascript thanks to emscripten

# API

syncronously compress the `in` buffer with pkware implode; will use the implode auto detect if dictSize is `undefined`
```ts
implode(in: Buffer, dictSize?)
```

syncronously decompress the `in` buffer with pkware explode
```ts
explode(in: Buffer)
```

calculate checksum
```ts
crc32(in: Buffer, xor?: boolean)
```

dictSize constants
```ts
ImplodeDictSize1
ImplodeDictSize2,
ImplodeDictSize3,
```


# Development

In your (windows) emscripten environment run `build/build.bat`