cmake_minimum_required(VERSION 3.5)
project (nc)

set(SOURCES
	atomicio.c
    netcat.c
    socks.c
)

add_executable(nc ${SOURCES})

target_link_libraries(nc tls ssl crypto)
