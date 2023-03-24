target_sources(${TARGET_ELF} PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/source/ch32v20x_it.c
    ${CMAKE_CURRENT_SOURCE_DIR}/source/core_riscv.c
    ${CMAKE_CURRENT_SOURCE_DIR}/source/startup_ch32v20x_D6.S
    ${CMAKE_CURRENT_SOURCE_DIR}/source/system_ch32v20x.c
    ${CMAKE_CURRENT_SOURCE_DIR}/source/debug.c
    ${CMAKE_CURRENT_SOURCE_DIR}/include/ch32v20x_conf.h
    ${CMAKE_CURRENT_SOURCE_DIR}/include/ch32v20x_it.h
    ${CMAKE_CURRENT_SOURCE_DIR}/include/core_riscv.h
    ${CMAKE_CURRENT_SOURCE_DIR}/include/system_ch32v20x.h
    ${CMAKE_CURRENT_SOURCE_DIR}/include/debug.h
)

target_include_directories(${TARGET_ELF} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)