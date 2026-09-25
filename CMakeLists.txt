cmake_minimum_required(VERSION 3.16)

project(cpp_hello_lab LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(cpp_hello_lab main.cpp)

include(GNUInstallDirs)
install(TARGETS cpp_hello_lab
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
    RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
)
