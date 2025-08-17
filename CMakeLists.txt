# Copyright (c) 2014 by AppSmiths Ventures LLP.  All Rights Reserved.
#
# All material is proprietary to AppSmiths Ventures LLP and may be used only
# pursuant to license rights granted by AppSmiths Ventures LLP  Other
# reproduction, distribution, or use is strictly prohibited.
#

cmake_minimum_required(VERSION 3.30)

###############
# ASI default settings
list(APPEND CMAKE_MODULE_PATH "$ENV{ASV_CMAKE}")
include(asv_cmake_defaults)
asv_cmake_defaults( )
###############

option(ZSTD_BUILD_CONTRIB "BUILD CONTRIB" OFF)
option(ZSTD_BUILD_STATIC "BUILD STATIC LIB" ON)
option(ZSTD_BUILD_SHARED "BUILD SHARED LIB" ON)

add_subdirectory(build/cmake)
