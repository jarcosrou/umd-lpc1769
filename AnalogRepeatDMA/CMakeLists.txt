cmake_minimum_required(VERSION 2.8.4)
set(CMAKE_TOOLCHAIN_FILE ../Platform/LPC1769.cmake)

project(AnalogRepeatDMA C)

set(SOURCES
 src/cr_startup_lpc176x.c
 src/analogrepeatdma.c
)

# Debug builds by default, uncomment for Release:
# set(CMAKE_RELEASE True)

# Uncomment to enable Semihosting (required to even link against
# semihosting libraries)
# set(SEMIHOSTING_ENABLED True)

include(../Platform/LPC1769_project_default.cmake)
include(../Platform/LPC1769_targets.cmake)
