add_subdirectory(googletest-release-1.7.0)

add_executable(CodeKataTests CodeKataTests.cpp $<TARGET_OBJECTS:CodeKata>)

target_include_directories(CodeKataTests PRIVATE ${gtest_SOURCE_DIR}/include ${PROJECT_SOURCE_DIR})

target_link_libraries(CodeKataTests gtest_main)