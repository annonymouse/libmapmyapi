add_subdirectory(gtest)

cmake_minimum_required (VERSION 3.1.0)
enable_testing()
include_directories(${GTEST_INCLUDE_DIRS})
add_executable(apitest apitest.cpp)
target_link_libraries(apitest ${GTEST_BOTH_LIBRARIES})
add_test(AllTestsInAPITest apitest)

