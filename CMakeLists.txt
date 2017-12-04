CMAKE_MINIMUM_REQUIRED (VERSION 2.6)
PROJECT (MYSKILLS) 
#自动定义了PROJECT_SOURCE_DIR 和 PROJECT_BINARY_DIR
#也自动定义了MYSKILLS_SOURCE_DIR 和 MYSKILLS_BINARY_DIR
#这目录是当前，如果在build下cmake，这目录就是build

#ADD_SUBDIRECTORY(src)
ADD_SUBDIRECTORY(src tmpbin)
#src是有源的子目录，tmpbin是编译结果(make时)存放地方
#现在这个外层目录什么文件都没用到，除了下面安装的目录参数

#ADD_EXECUTABLE(myskills ${SRC_LIST})

SET(CMAKE_INSTALL_PREFIX "/usr/local/test/")

#INSTALL (TARGETS myskills DESTINATION installbin)
