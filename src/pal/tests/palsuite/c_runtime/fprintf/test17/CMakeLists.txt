cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  test17.c
)

add_executable(paltest_fprintf_test17
  ${SOURCES}
)

add_dependencies(paltest_fprintf_test17 CoreClrPal)

target_link_libraries(paltest_fprintf_test17
  pthread
  m
  CoreClrPal
)
