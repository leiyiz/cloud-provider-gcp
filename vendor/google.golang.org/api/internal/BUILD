load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "conn_pool.go",
        "creds.go",
        "settings.go",
    ],
    importmap = "k8s.io/cloud-provider-gcp/vendor/google.golang.org/api/internal",
    importpath = "google.golang.org/api/internal",
    visibility = ["//vendor/google.golang.org/api:__subpackages__"],
    deps = [
        "//vendor/golang.org/x/oauth2:go_default_library",
        "//vendor/golang.org/x/oauth2/google:go_default_library",
        "//vendor/google.golang.org/api/internal/impersonate:go_default_library",
        "//vendor/google.golang.org/grpc:go_default_library",
    ],
)
