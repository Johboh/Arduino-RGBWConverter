
FILE(GLOB_RECURSE sources "./src/*.*")

set(required_components arduino-esp32)

idf_component_register(COMPONENT_NAME "arduino_rgbwconverter"
                        SRCS ${sources}
                        INCLUDE_DIRS "./src/"
                        REQUIRES ${required_components})
