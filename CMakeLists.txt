cmake_minimum_required(VERSION 3.10)
project(DataStructureWebsite)

# Set the vcpkg toolchain file
set(CMAKE_TOOLCHAIN_FILE "${CMAKE_SOURCE_DIR}/gtest/vcpkg/scripts/buildsystems/vcpkg.cmake" CACHE STRING "Vcpkg toolchain file")

# Add subdirectories
add_subdirectory(DataStructureWebsiteComponent/UnitTests)

# Running Unit Tests:

# When making changes to cmake file, run this command
# cd ~/DataStructureWebsite/Build
# cmake -DCMAKE_TOOLCHAIN_FILE=../Gtest/vcpkg/scripts/buildsystems/vcpkg.cmake ..


# When making changes to only the source code, run this command 
# cd ~/DataStructureWebsite/Build
# cmake --build .