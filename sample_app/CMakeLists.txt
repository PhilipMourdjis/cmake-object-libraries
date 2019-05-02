# Sample executable that links against "core"
add_executable(sample_app sample_app.cpp)
target_link_libraries(sample_app PRIVATE core)