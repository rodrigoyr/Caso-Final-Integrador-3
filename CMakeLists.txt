cmake_minimum_required(VERSION 3.26)
project(Caso_Final_Integrador_3)

set(CMAKE_CXX_STANDARD 17)


add_executable(Caso_Final_Integrador_3 main.cpp)




cmake_minimum_required(VERSION 3.15)
project(BoostExample)

set(CMAKE_CXX_STANDARD 14)

set(BOOST_ROOT "path/to/your/boost")

find_package(Boost 1.75.0)

if(Boost_FOUND)
    include_directories(${Boost_INCLUDE_DIRS})
    add_executable(BoostExample main.cpp)
    target_link_libraries(BoostExample ${Boost_LIBRARIES})
endif()