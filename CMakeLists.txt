cmake_minimum_required(VERSION 3.10)
project(MiniShell)

# 指定 C++ 標準
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# 包含標頭檔路徑
include_directories(include)

# 收集原始碼檔案
file(GLOB SOURCES "src/*.cpp")

# 定義可執行檔
add_executable(minishell ${SOURCES})
