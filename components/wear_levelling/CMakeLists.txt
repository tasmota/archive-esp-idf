idf_component_register(SRCS "Partition.cpp"
                            "SPI_Flash.cpp"
                            "WL_Ext_Perf.cpp"
                            "WL_Ext_Safe.cpp"
                            "WL_Flash.cpp"
                            "crc32.cpp"
                            "wear_levelling.cpp"
                    INCLUDE_DIRS include
                    PRIV_INCLUDE_DIRS private_include
                    REQUIRES spi_flash)

target_compile_options(${COMPONENT_LIB} PRIVATE "-Wno-format")
