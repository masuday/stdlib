ADDTEST(mean)

if(DEFINED CMAKE_MAXIMUM_RANK)
    if(${CMAKE_MAXIMUM_RANK} GREATER 7)
        ADDTEST(mean_f03)
    endif()
elseif(f03rank)
    ADDTEST(mean_f03)
endif()
