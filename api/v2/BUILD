load("@com_github_grpc_grpc//bazel:python_rules.bzl", "py_proto_library", "py_grpc_library")
load("@rules_proto//proto:defs.bzl", "proto_library")

proto_library(
    name = "api_proto",
    srcs = ["api.proto"],
)

py_proto_library(
    name = "api_py_pb2",
    deps = [":api_proto"],
)

py_grpc_library(
    name = "api_py_pb2_grpc",
    srcs = [":api_proto"],
    deps = [":api_py_pb2"],
)
