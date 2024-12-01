add_library(calc_lib STATIC calc.h calc.cpp)

target_link_libraries(calc_lib PUBLIC converter_lib)
target_link_libraries(calc_lib PUBLIC stack_lib)

target_include_directories(calc_lib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})