cmake_minimum_required(VERSION 3.10)
project(poker-ai)

set(CMAKE_CXX_STANARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED TRUE)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_compile_definitions(${PROJECT_NAME} BASE_PATH="${CMAKE_SOURCE_DIR}/")

add_executable(${PROJECT_NAME} src/main.cpp)

target_include_directories(${PROJECT_NAME}
	PRIVATE src/
)
