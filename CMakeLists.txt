cmake_minimum_required(VERSION 2.8.5)

project(MLPractice)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

set(EXTERNAL_DIR "${CMAKE_CURRENT_SOURCE_DIR}/external")
set(EIGEN_INCLUDE_DIR "${EXTERNAL_DIR}/eigen-3.3.7")

add_executable(PCA 
    LinearAlgebra/PCA.cpp
    )

target_include_directories(PCA
    PRIVATE ${EIGEN_INCLUDE_DIR}
    )
