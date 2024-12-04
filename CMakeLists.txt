zephyr_library()

zephyr_interface_library_named(sh2)

zephyr_include_directories(sh2 INTERFACE
  ${ZEPHYR_BASE}/include
  .
  )

zephyr_library_link_libraries(sh2)

zephyr_library_sources(
    euler.c
    sh2.c
    sh2_util.c
    shtp.c
    sh2_SensorValue.c
)
