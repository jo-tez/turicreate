project(sgraph_test)

make_boost_test(hilbert_par_for.cxx REQUIRES unity_shared_for_testing)
make_boost_test(sgraph_test.cxx REQUIRES unity_shared_for_testing)
make_boost_test(sgraph_vertex_apply_test.cxx REQUIRES unity_shared_for_testing)
make_boost_test(sgraph_engine_test.cxx REQUIRES unity_shared_for_testing)
make_boost_test(sgraph_triple_apply_test.cxx REQUIRES unity_shared_for_testing)
make_boost_test(sgraph_fast_triple_apply_test.cxx REQUIRES unity_shared_for_testing)
make_executable(sgraph_bench SOURCES sgraph_bench.cpp REQUIRES unity_shared_for_testing)
