add_executable(${PROJECT_NAME}
  arsenal.for
  cornelius2.f90
  eos.for
  initialization.for
  input_function.for
  phy_boundary.for
  Jetoutputh5.for
  util.for
  vishnew.for
)

target_link_libraries(${PROJECT_NAME} ${HDF5_LIBRARIES})

install(TARGETS ${PROJECT_NAME} DESTINATION bin)
