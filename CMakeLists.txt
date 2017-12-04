project(particle_filter)

#cmake_minimum_required(VERSION 2.8)

FIND_PACKAGE(OpenCV REQUIRED)

add_executable(particle_filter ./src/particle_filter.cpp)

target_link_libraries(particle_filter ${OpenCV_LIBS})

install(TARGETS particle_filter 
DESTINATION ${PROJECT_SOURCE_DIR}/bin)
