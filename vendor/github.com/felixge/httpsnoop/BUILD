load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "capture_metrics.go",
        "docs.go",
        "wrap_generated_gteq_1.8.go",
        "wrap_generated_lt_1.8.go",
    ],
    importmap = "k8s.io/cloud-provider-gcp/vendor/github.com/felixge/httpsnoop",
    importpath = "github.com/felixge/httpsnoop",
    visibility = ["//visibility:public"],
)
