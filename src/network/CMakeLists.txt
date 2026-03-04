
set(MODULE_NAME network)

# add_subdirectory(api2.0.3)
add_subdirectory(api_wm)
# add_subdirectory(lwip2.0.3)
add_subdirectory(lwip2.1.3)

add_library(${MODULE_NAME} INTERFACE)

target_link_libraries(${MODULE_NAME} INTERFACE api_wm lwip2.1.3)
# target_link_libraries(${MODULE_NAME} INTERFACE api2.1.3 lwip2.1.3)
