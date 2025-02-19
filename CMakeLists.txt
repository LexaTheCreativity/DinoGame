cmake_minimum_required(VERSION 3.0)
project(DinoGame)

set(CMAKE_CXX_STANDARD 17)  # Use modern C++

# Find SFML
find_package(SFML 2.5 COMPONENTS graphics window system REQUIRED)

# Add the executable
add_executable(dino_game src/main.cpp)

# Link SFML libraries
target_link_libraries(dino_game sfml-graphics sfml-window sfml-system)
