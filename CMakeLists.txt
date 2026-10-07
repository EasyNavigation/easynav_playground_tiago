cmake_minimum_required(VERSION 3.20)
project(easynav_playground_tiago)

find_package(ament_cmake REQUIRED)

install(DIRECTORY
  launch
  config
  maps
  params
  rviz
  urdf
  meshes
  worlds
  models
  photos
  DESTINATION share/${PROJECT_NAME}
)

install(FILES LICENSE DESTINATION share/${PROJECT_NAME})

ament_package()
