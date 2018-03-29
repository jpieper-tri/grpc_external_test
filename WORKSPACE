workspace(name = "grpc_external_test")

http_archive(
    name = "com_github_grpc_grpc",
    url = "https://github.com/jpieper-tri/grpc/archive/2d91511e50d1793826d8f3f3d599f7ad0b476222.tar.gz",
    strip_prefix = "grpc-2d91511e50d1793826d8f3f3d599f7ad0b476222",
)

bind(
    name = "grpc_cpp_plugin",
    actual = "@com_github_grpc_grpc//:grpc_cpp_plugin",
)

bind(
    name = "grpc++_codegen_proto",
    actual = "@com_github_grpc_grpc//:grpc++_codegen_proto",
)

load("@com_github_grpc_grpc//bazel:grpc_deps.bzl", "grpc_deps")

grpc_deps()
