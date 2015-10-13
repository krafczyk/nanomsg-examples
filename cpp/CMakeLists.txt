add_definitions(-std=c++11)

add_executable(pipeline_cpp pipeline.cpp)
target_link_libraries(pipeline_cpp ${libnanomsg_LDFLAGS})

add_executable(reqrep_cpp reqrep.cpp)
target_link_libraries(reqrep_cpp ${libnanomsg_LDFLAGS})

add_executable(pair_cpp pair.cpp)
target_link_libraries(pair_cpp ${libnanomsg_LDFLAGS})

add_executable(pubsub_cpp pubsub.cpp)
target_link_libraries(pubsub_cpp ${libnanomsg_LDFLAGS})

add_executable(survey_cpp survey.cpp)
target_link_libraries(survey_cpp ${libnanomsg_LDFLAGS})

add_executable(bus_cpp bus.cpp)
target_link_libraries(bus_cpp ${libnanomsg_LDFLAGS})

install (TARGETS pipeline_cpp reqrep_cpp pair_cpp pubsub_cpp survey_cpp bus_cpp DESTINATION bin)
