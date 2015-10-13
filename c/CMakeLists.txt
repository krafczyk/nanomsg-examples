add_executable(pipeline_c pipeline.c)
target_link_libraries(pipeline_c ${libnanomsg_LDFLAGS})

add_executable(reqrep_c reqrep.c)
target_link_libraries(reqrep_c ${libnanomsg_LDFLAGS})

add_executable(pair_c pair.c)
target_link_libraries(pair_c ${libnanomsg_LDFLAGS})

add_executable(pubsub_c pubsub.c)
target_link_libraries(pubsub_c ${libnanomsg_LDFLAGS})

add_executable(survey_c survey.c)
target_link_libraries(survey_c ${libnanomsg_LDFLAGS})

add_executable(bus_c bus.c)
target_link_libraries(bus_c ${libnanomsg_LDFLAGS})

install (TARGETS pipeline_c reqrep_c pair_c pubsub_c survey_c bus_c DESTINATION bin)
