message(STATUS "add lite kernels")

set(lite_kernel_deps type_system kernel op op_registry context tensor any CACHE INTERNAL "" FORCE)

add_subdirectory(host)
add_subdirectory(arm)
add_subdirectory(cuda)
add_subdirectory(x86)
add_subdirectory(opencl)
add_subdirectory(fpga)
add_subdirectory(npu)
add_subdirectory(xpu)
add_subdirectory(mlu)
add_subdirectory(bm)
