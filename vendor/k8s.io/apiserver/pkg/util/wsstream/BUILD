load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "conn.go",
        "doc.go",
        "stream.go",
    ],
    importpath = "k8s.io/apiserver/pkg/util/wsstream",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/golang/glog:go_default_library",
        "//vendor/golang.org/x/net/websocket:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/runtime:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
