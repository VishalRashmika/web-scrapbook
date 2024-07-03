+++
title = "Raylib"
date = 2024-07-03
+++

## Raylib command (linux)

```
g++ main.cpp -lraylib -lGL -lm -lpthread -ldl -lrt -lX11 -o main && ./main
```

# Raylib starter template for windows

- [Raylib Starter Template](https://scrapbook.vishalrashmika.com/raylib.zip)

# Raylib to web-assembly (windows)
```
emcc -o ./export/pong.html ./src/main.cpp -Wall -std=c++14 -D_DEFAULT_SOURCE -Wno-missing-braces -Wunused-result -Os -I. -I C:/raylib/raylib/src -I C:/raylib/raylib/src/external -L. -L C:/raylib/raylib/src -s USE_GLFW=3 -s ASYNCIFY -s TOTAL_MEMORY=67108864 -s FORCE_FILESYSTEM=1 --shell-file C:/raylib/raylib/src/shell.html C:/raylib/raylib/src/web/libraylib.a -DPLATFORM_WEB -s 'EXPORTED_FUNCTIONS=["_free","_malloc","_main"]'-s EXPORTED_RUNTIME_METHODS=ccall
```