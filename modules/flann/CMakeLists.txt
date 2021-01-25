set(the_description "Clustering and Search in Multi-Dimensional Spaces")
ocv_define_module(flann opencv_core WRAP python)

# MB patch begin
# FLANN module requires RTTI
target_compile_options( opencv_flann PRIVATE ${TNUN_compiler_rtti_on} )
# MB patch end
