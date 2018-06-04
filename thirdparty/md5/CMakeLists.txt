add_library (md5_bundled STATIC EXCLUDE_FROM_ALL
    md5.c
)


set_property(TARGET md5_bundled PROPERTY POSITION_INDEPENDENT_CODE ON)
