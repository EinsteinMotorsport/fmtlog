add_executable(log_test log_test.cc)
target_include_directories(log_test PRIVATE ${PROJECT_SOURCE_DIR}/include)
target_link_libraries(log_test fmtlog fmt pthread)

add_executable(enc_dec_test enc_dec_test.cc)
target_include_directories(enc_dec_test PRIVATE ${PROJECT_SOURCE_DIR}/include)
target_link_libraries(enc_dec_test fmtlog fmt pthread)

add_executable(multithread_test multithread_test.cc)
target_include_directories(multithread_test PRIVATE ${PROJECT_SOURCE_DIR}/include)
target_link_libraries(multithread_test fmt pthread)
