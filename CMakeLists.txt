cmake_minimum_required (VERSION 2.8)

# Can name the project whatever you want here
project(cmake_is_life)

# This points to where your headers will be (./include/ in this case)
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)

# Here we create the executable and tell it
# where to find the .c files it needs
add_executable(${PROJECT_NAME} src/main.c)

# Here we link any external libraries we want to use. For example,
# if you use math.h, you would normally use -lm in your compile
# command to link it. For this, the equivalent would be:

# target_link_libraries(${PROJECT_NAME} m)
