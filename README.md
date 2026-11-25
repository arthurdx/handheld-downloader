# handheld-dl

A download manager for RK3326 handhelds (R36H and similar). C++17, SDL2.

## Build

```sh
# Debian/Ubuntu: sudo apt install build-essential cmake libsdl2-dev
# Arch: sudo pacman -S --needed base-devel cmake ninja sdl2-compat
cmake -B build && cmake --build build
./build/handheld-dl
```
