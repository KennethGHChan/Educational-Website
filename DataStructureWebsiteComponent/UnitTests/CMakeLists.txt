cmake_minimum_required(VERSION 3.10)
project(UnitTests)

# Add the Backend directory
add_subdirectory(../Backend Backend_build)

# Find GTest
find_package(GTest REQUIRED)

# Add the executable for the tests
add_executable(MyBackendTests test_Stack.cpp)

# Link the executable to GTest and the Backend library
target_link_libraries(MyBackendTests GTest::gtest GTest::gtest_main MyBackend)
./