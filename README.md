# Space Invaders Game (C++ | OpenGL)

This is a simple 2D **Space Invaders** clone built using modern C++ and the OpenGL graphics pipeline.  
The project uses the **GLFW** library for window/context creation and input, and **GLEW** for loading OpenGL extensions.

---

## 🚀 Features

- OpenGL context creation using GLFW
- Extension loading with GLEW
- Game loop structure with input handling
- Clear code layout with debug options (GL error logging)
- CMake build system with DLL post-build copying

---

## 🧱 Dependencies

- [GLFW 3.4](https://www.glfw.org/download.html) 
- [GLEW 2.1.0](http://glew.sourceforge.net/)
- OpenGL (provided via Windows SDK)

---


---

## 🔧 Requirements

- [MinGW-w64](https://www.mingw-w64.org/) toolchain (used with CLion)
- [GLFW 3.4](https://www.glfw.org/)
- [GLEW 2.1.0](http://glew.sourceforge.net/)
- OpenGL-capable graphics hardware

---

## 📦 Library Setup

| Library | Header Path                                | Library File Path                                       | DLL (if needed)                                      |
|--------:|---------------------------------------------|----------------------------------------------------------|------------------------------------------------------|
| GLEW    | `D:/GLEW32_CPP/mingw64/include`            | `D:/GLEW32_CPP/mingw64/lib/libglew32.a`                 | `D:/GLEW32_CPP/mingw64/bin/glew32.dll`              |
| GLFW    | `D:/glfw-3.4.bin.WIN64/include`            | `D:/glfw-3.4.bin.WIN64/lib-mingw-w64/libglfw3.a`        | `D:/glfw-3.4.bin.WIN64/lib-mingw-w64/glfw3.dll`     |

---

## 🛠️ Build Instructions (CLion on Windows)

1. Open the project folder in **CLion**
2. Ensure the `CMakeLists.txt` has correct paths (already configured)
3. Use **Build → Rebuild Project**
4. Output executable: `cmake-build-debug/Space_Invaders_Game.exe`

DLLs are auto-copied post-build to the same folder using CMake commands.

---

## 🧪 Controls

| Key     | Action            |
|---------|-------------------|
| ← / →   | Move ship         |
| Space   | Fire (planned)    |
| ESC     | Close the window  |

---


## 📄 License

This project is licensed under the **MIT License**.  
Feel free to use, modify, and distribute the code.

---

## 🙏 Credits

- [GLFW](https://www.glfw.org/)
- [GLEW](http://glew.sourceforge.net/)
- [OpenGL](https://www.khronos.org/opengl/)

---

## 🤝 Contributions

Want to improve movement, add sprites, or enemy waves?  
PRs and forks are welcome!


