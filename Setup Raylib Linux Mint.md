# Setup Raylib in Linux Mint

```bash
sudo apt install libx11-dev libxcursor-dev libxinerama-dev   libxi-dev  libx11-dev libglu1-mesa-dev libxrandr-dev
```

```bash
mv game-premake game_name
```

```bash
git clone https://github.com/raylib-extras/game-premake.git --depth 1
```
```bash
mv game-premake game_name
```

```bash
cd game_name
```

### Need to run this every time you add or remove file in src folder
```bash
./premake5 gmake
```

```bash
make
```

### To run the game
```bash
./_bin/Debug/game_name
```

### Reference

 - [https://github.com/albertnadal/MandelbrotGoLang/issues/1]

