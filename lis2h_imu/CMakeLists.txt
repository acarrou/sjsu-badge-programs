add_executable(lis2h_imu
        lis2h_imu.c
        )

# pull in common dependencies and additional i2c hardware support
target_link_libraries(lis2h_imu pico_stdlib hardware_i2c)

# create map/bin/hex file etc.
pico_add_extra_outputs(lis2h_imu)

# add url via pico_set_program_url
example_auto_set_url(lis2h_imu)
