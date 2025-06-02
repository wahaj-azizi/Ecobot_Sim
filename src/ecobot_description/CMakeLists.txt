cmake_minimum_required(VERSION 3.5)
project(ecobot_description)

find_package(ament_cmake REQUIRED)

install(DIRECTORY
  meshes
  DESTINATION share/${PROJECT_NAME}
)

install(FILES
  Ecobot.urdf
  DESTINATION share/${PROJECT_NAME}
)


install(
  DIRECTORY launch
  DESTINATION share/${PROJECT_NAME}/
)

ament_package()
