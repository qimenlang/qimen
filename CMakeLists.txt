# CMakeList.txt: Engine 的 CMake 项目，在此处包括源代码并定义
# 项目特定的逻辑。
#
cmake_minimum_required (VERSION 3.15)

project ("Engine")

# 将源代码添加到此项目的可执行文件。
add_executable (Engine "Engine.cpp" "Engine.h")

add_subdirectory(thirdparty)

target_link_libraries(Engine PUBLIC glfw glad)

# TODO: 如有需要，请添加测试并安装目标。
