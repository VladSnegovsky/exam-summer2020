set(LIB_NAME ${PROJECT_NAME}core)

set(SRC_LIST
		trees/AVLtree.hpp
		trees/AVLtree.tpp
        
        sortings/Change.hpp
        sortings/Sort.hpp
        sortings/Type.hpp
		sortings/RadixSort.hpp

        trees/splay_set.hpp
        trees/splay_map.hpp
		trees/BplusTree.hpp
        trees/BplusTree.tpp
		trees/BTree.hpp
		trees/BTree.tpp


        lists/DLsircular.hpp
        lists/DLsircular.tpp
		lists/SL.hpp
		lists/SLsircular.tpp lists/SLsircular.hpp
		
		types/Official.hpp
		types/Official.cpp
		)

add_library(${LIB_NAME} STATIC ${SRC_LIST})

set_target_properties(${LIB_NAME} PROPERTIES LINKER_LANGUAGE CXX)
