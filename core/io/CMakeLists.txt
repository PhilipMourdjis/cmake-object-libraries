# OBJECT LIBRARY
add_library(core_io_obj OBJECT
            private/io.cpp)

target_include_directories(core_io_obj PUBLIC ${PROJECT_SOURCE_DIR})
target_compile_definitions(core_io_obj PRIVATE COMPILING_DLL)

# REGULAR LIBRARY (explicitly SHARED)
# Note: some IDEs may not show the target if the target has no sources itself. 
add_library(core_io STATIC)

target_link_libraries(core_io PUBLIC core_io_obj)

