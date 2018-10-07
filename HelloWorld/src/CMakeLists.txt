cmake_minimum_required(VERSION 3.0)
# Name our project
project (hello_example)

# add all the *.c files as sources
FILE(GLOB SRC_FILES *.c)

# hello below is the name of the binary generated
add_executable(hello ${SRC_FILES})

# use below link libararies if you want to link 3 party libraries and other built local projects
target_link_libraries(hello
#pthread
#jsoncpp
#curl
#${Boost_LIBRARIES}
)

#add below command if you have folders inside src which needs to be complied.
#make sure the new folder contains CMakeList.txt files along with src code.
#add_subdirectory(driver)

#include directories if needed
#include_directories(${CMAKE_SYSROOT}/usr/include)

#find packages when required
#find_package(Boost REQUIRED COMPONENTS date_time)