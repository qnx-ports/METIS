add_executable(mtest mtest.c)

target_link_libraries(mtest metis) 
target_include_directories(mtest PRIVATE ${CMAKE_SOURCE_DIR}/libmetis)
if(METIS_INSTALL)
  install(TARGETS mtest
    RUNTIME DESTINATION bin/metis_tests)
endif()
