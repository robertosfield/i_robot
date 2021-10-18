set(SOURCES
   main.cpp
)

add_executable(basic_scene ${SOURCES})

target_link_libraries(basic_scene vsg::vsg)

if (vsgXchange_FOUND)
    target_compile_definitions(basic_scene PRIVATE vsgXchange_FOUND)
    target_link_libraries(basic_scene vsgXchange::vsgXchange)
endif()

install(TARGETS basic_scene RUNTIME DESTINATION bin)
