if(METIS_INSTALL)
  if(QNX)
    install(FILES metis.h DESTINATION ${CMAKE_INSTALL_INCLUDEDIR})
  else()
    install(FILES metis.h DESTINATION include)
  endif()
endif()
