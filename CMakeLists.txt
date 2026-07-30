cmake_minimum_required(VERSION 3.16)

set(COMPONENT_SRCDIRS
        src/
        )

set(COMPONENT_REQUIRES
        driver
        esp_driver_gpio
        esp_driver_gptimer
        )

set(COMPONENT_ADD_INCLUDEDIRS
        src/
        )

idf_component_register(
        SRC_DIRS ${COMPONENT_SRCDIRS}
        REQUIRES ${COMPONENT_REQUIRES}
        INCLUDE_DIRS ${COMPONENT_ADD_INCLUDEDIRS}
)