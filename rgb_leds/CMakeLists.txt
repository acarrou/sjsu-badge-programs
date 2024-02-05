add_executable(rgb_leds
        rgb_leds.c
        )

# pull in common dependencies
target_link_libraries(rgb_leds pico_stdlib)

# create map/bin/hex file etc.
pico_add_extra_outputs(rgb_leds)

# add url via pico_set_program_url
example_auto_set_url(rgb_leds)
