if(IDF_VERSION_MAJOR GREATER_EQUAL 4)
    idf_component_register(SRC_DIRS .
        INCLUDE_DIRS include)
else()
    set(COMPONENT_SRCDIRS .)
    set(COMPONENT_ADD_INCLUDEDIRS include)
    register_component()
endif()
