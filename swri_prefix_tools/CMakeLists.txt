cmake_minimum_required(VERSION 2.8.3)
project(swri_prefix_tools)

find_package(catkin REQUIRED)
catkin_package()

catkin_install_python(PROGRAMS xterm_prefix
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
install(PROGRAMS xterm_prefix_callgrind
                 xterm_prefix_callgrind_wait
                 xterm_prefix_gdb
                 xterm_prefix_hold
                 xterm_prefix_normal
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
