add_executable(${PROJECT_NAME}
  arsenal.for
  cornelius2.f90
  initialization.for
  input_eos.for
  input_function.for
  oscar_output.for
  phy_boundary.for
  vishnew.for
  jet_output_hdf5.for
  util.for
)

target_link_libraries(${PROJECT_NAME} ${HDF5_LIBRARIES})


install(TARGETS ${PROJECT_NAME} DESTINATION bin)
