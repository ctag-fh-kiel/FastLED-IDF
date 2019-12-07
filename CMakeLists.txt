idf_component_register(SRCS FastLED.cpp		colorpalettes.cpp	hsv2rgb.cpp		noise.cpp		power_mgt.cpp
bitswap.cpp		colorutils.cpp		lib8tion.cpp		platforms.cpp		wiring.cpp
                       INCLUDE_DIRS "."
                       REQUIRES mbedtls)
add_definitions(-DESP32)
target_compile_options(${COMPONENT_LIB} PRIVATE -Wno-error=class-memaccess)