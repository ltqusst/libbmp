PROJECT(bmplib)
CMAKE_MINIMUM_REQUIRED(VERSION 2.8)

include_directories(${CMAKE_SOURCE_DIR})

ADD_LIBRARY(bmp	SHARED libbmp.c)
TARGET_LINK_LIBRARIES(bmp m)

INSTALL(TARGETS bmp        DESTINATION "lib")
INSTALL(FILES libbmp.h    DESTINATION "include")

ADD_EXECUTABLE(test_libbmp 	test.c)
TARGET_LINK_LIBRARIES(test_libbmp bmp)

