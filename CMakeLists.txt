
#1.设置最低版本
cmake_minimum_required(VERSION 2.8)
#SET(CMAKE_C_COMPILER g++)

#CMAKE_FORCE_C_COMPILER(gcc GNU)
#CMAKE_FORCE_CXX_COMPILER(g++ GNU)
#2.添加编译选项
add_compile_options(-std=c++11)
#3.设置项目
project(xmlconfig)
#4.添加源文件
aux_source_directory(. DIR_SRCS)

include_directories(.)
#5.链接三方库
#link_libraries(xml2)
#6.生成可执行文件
add_executable(xmlconfigtest ${DIR_SRCS})