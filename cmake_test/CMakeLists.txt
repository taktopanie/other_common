cmake_minimum_required(VERSION 3.10)
project(MyProgram)

# Add include directory for your custom library
include_directories(${CMAKE_SOURCE_DIR}/lib)

# Add link directory for your custom library
link_directories(${CMAKE_SOURCE_DIR}/lib)

# Add the executable target
add_executable(program.exe main.c)

# Link with your custom library 'libMY'
# This assumes you have libMY.a or libMY.so in ./lib/
link_directories(${CMAKE_SOURCE_DIR}/lib)
target_link_libraries(program.exe MY)
