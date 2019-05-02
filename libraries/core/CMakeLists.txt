add_subdirectory(database)
add_subdirectory(io)

# CORE library that combines the two libraries (database and io)
add_library(core SHARED)
target_link_libraries(core PUBLIC core_io_obj core_database_obj)

