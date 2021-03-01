include_directories(${hw2_INCDIR})

add_executable(test_vpn test_vpn.cpp)
target_link_libraries(test_vpn hw2 googletest )
add_test(ExtractVPN ./test_vpn)

add_executable(test_pfn test_pfn.cpp)
target_link_libraries(test_pfn hw2 googletest )
add_test(PFNtoAddr ./test_pfn)

add_executable(test_tlb test_tlb.cpp)
target_link_libraries(test_tlb hw2 googletest )
add_test(TLBLookup ./test_tlb)

add_executable(test_table test_table.cpp)
target_link_libraries(test_table hw2 googletest )
add_test(PageTableLookup ./test_table)



add_executable(test_fifo test_fifo.cpp)
target_link_libraries(test_fifo hw2 googletest)
add_test(FIFOTest ./test_fifo)

add_executable(test_lru test_lru.cpp)
target_link_libraries(test_lru hw2 googletest)
add_test(LRUTest ./test_lru)

add_executable(test_clock_lru test_clock_lru.cpp)
target_link_libraries(test_clock_lru hw2 googletest)
add_test(ClockLRUTest ./test_clock_lru)

