cmake_minimum_required(VERSION 3.10)

project(CI_CD VERSION 1.1)

add_executable(main main.cpp statistics.cpp)

enable_testing()
add_executable(test_statistics statistics.cpp test_statistics.cpp)
add_test(NAME StatisticsTests COMMAND test_statistics)
