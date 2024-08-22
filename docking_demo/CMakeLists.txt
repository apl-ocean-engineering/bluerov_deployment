cmake_minimum_required(VERSION 3.8)
project(docking_demo)

find_package(ament_cmake REQUIRED)

install(
  DIRECTORY control_integration/launch
            control_integration/config
  DESTINATION share/docking_demo/control_integration
)

install(
  DIRECTORY teleoperation/launch
            teleoperation/config
  DESTINATION share/docking_demo/teleoperation
)

ament_package()
