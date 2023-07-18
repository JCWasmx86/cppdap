cppdap_deps = [meson.get_compiler('cpp').find_library('jsoncpp')]
cppdap_lib = library(
    'cppdap',
    'content_stream.cpp',
    'io.cpp',
    'jsoncpp_json_serializer.cpp',
    'network.cpp',
    'null_json_serializer.cpp',
    'protocol_events.cpp',
    'protocol_requests.cpp',
    'protocol_response.cpp',
    'protocol_types.cpp',
    'session.cpp',
    'socket.cpp',
    'typeinfo.cpp',
    'typeof.cpp',
    cpp_args: ['-DCPPDAP_JSON_JSONCPP=1'],
    dependencies: cppdap_deps,
    include_directories: inc,
)

cppdap_dep = declare_dependency(
    dependencies: cppdap_deps,
    include_directories: inc,
    link_with: [cppdap_lib],
)


