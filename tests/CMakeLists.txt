add_subdirectory(googletest-release-1.7.0)

include_directories(${gtest_SOURCE_DIR}/include)

add_executable(CodeKataTests CodeKataTests.cpp $<TARGET_OBJECTS:CodeKata>)

target_link_libraries(CodeKataTests gtest_main)