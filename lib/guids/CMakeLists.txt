add_library (guids STATIC
    guids.cpp
    guids_defs.hpp
    guids_entries.h
    guids.hpp
)

set_property(TARGET guids PROPERTY POSITION_INDEPENDENT_CODE ON)

add_gtest (guids_test guids_test.cpp)
target_link_libraries (guids_test guids)
