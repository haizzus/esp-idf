
set(COMPONENT_SRCS
                    "light_driver.c"
                    "iot_led.c"
                    "led_strip_encoder.c")

set(COMPONENT_ADD_INCLUDEDIRS ". include")

# requirements can't depend on config
set(COMPONENT_REQUIRES example_nvs driver esp_driver_gpio esp_driver_ledc)

register_component()
