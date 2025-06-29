cmake_minimum_required(VERSION 3.31)
project(Space_Invaders_Game)

set(CMAKE_CXX_STANDARD 20)

add_executable(Space_Invaders_Game main.cpp)

# === Include paths ===
include_directories(
        "D:/GLEW32_CPP/mingw64/include"
        "D:/glfw-3.4.bin.WIN64/include"
)

# === Link paths (for *.a static libraries) ===
target_link_libraries(Space_Invaders_Game
        "D:/GLEW32_CPP/mingw64/lib/libglew32.a"
        "D:/glfw-3.4.bin.WIN64/lib-mingw-w64/libglfw3.a"
        opengl32
)


# === Libraries (match file names: libglew32.a, libglfw3.a) ===
target_link_libraries(Space_Invaders_Game
        glew32
        glfw3
        opengl32
)

# === (Optional) Copy runtime DLLs — safe even for static link ===
add_custom_command(TARGET Space_Invaders_Game POST_BUILD
        COMMAND ${CMAKE_COMMAND} -E copy_if_different
        "D:/GLEW32_CPP/mingw64/bin/glew32.dll"
        "D:/glfw-3.4.bin.WIN64/lib-mingw-w64/glfw3.dll"
        $<TARGET_FILE_DIR:Space_Invaders_Game>
)
