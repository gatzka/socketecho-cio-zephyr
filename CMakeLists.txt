# SPDX-License-Identifier: Apache-2.0

cmake_minimum_required(VERSION 3.13.1)
set(CIO_BUILD_FOR_ZEPHYR ON)

include($ENV{ZEPHYR_BASE}/cmake/app/boilerplate.cmake NO_POLICY_SCOPE)
project(socket_echo_cio)

target_sources(app PRIVATE src/socket_echo.c)
target_link_libraries (app PUBLIC cio::cio)
