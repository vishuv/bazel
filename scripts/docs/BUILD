filegroup(
    name = "srcs",
    srcs = glob(["**"]),
    visibility = ["//scripts:__pkg__"],
)

py_library(
    name = "dot-converter",
    srcs = ["dot_converter.py"],
)

py_binary(
    name = "generate_dot_graphs",
    srcs = ["generate_dot_graphs.py"],
    data = ["@dot//:cmd/dot/dot"],
    tags = ["manual"],
    visibility = ["//site:__pkg__"],
    deps = [":dot-converter"],
)
