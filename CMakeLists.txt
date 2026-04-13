
FILE(GLOB_RECURSE sources "./src/*.*")

idf_component_register(COMPONENT_NAME "arduino_rgbwconverter"
                        SRCS ${sources}
                        INCLUDE_DIRS "./src/")
