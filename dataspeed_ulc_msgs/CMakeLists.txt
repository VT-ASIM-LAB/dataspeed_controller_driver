cmake_minimum_required(VERSION 3.0.2)
project(dataspeed_ulc_msgs)

find_package(catkin REQUIRED COMPONENTS
  message_generation
  std_msgs
)

add_message_files(
  DIRECTORY
    msg
  FILES
    UlcCmd.msg
    UlcReport.msg
)

generate_messages(
DEPENDENCIES
  std_msgs
)

catkin_package()
