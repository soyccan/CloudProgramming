project('chord', 'cpp',
        default_options: ['cpp_std=c++20'])

cmake = import('cmake')
rpclib_proj = cmake.subproject('rpclib')
rpclib_dep = rpclib_proj.dependency('rpc') # librpc

executable(
    'chord',
    'src/chord.cc',
    dependencies: [rpclib_dep]
)
