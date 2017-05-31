project('cpr', 'cpp', version : '1.3.0', license : 'MIT')

curl_dep = dependency('libcurl')

comp_flags=['-std=c++14']
link_flags=['-lpthread']

includes = include_directories('include')
subdir('cpr')

cpr_lib = shared_library('cpr', include_directories: includes, sources: cpr_src, dependencies: curl_dep)
cpr_dep = declare_dependency(include_directories: includes, link_with: cpr_lib)
