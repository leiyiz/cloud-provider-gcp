load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "log_level.go",
        "zap.go",
        "zap_journal.go",
    ],
    importmap = "k8s.io/cloud-provider-gcp/vendor/go.etcd.io/etcd/client/pkg/v3/logutil",
    importpath = "go.etcd.io/etcd/client/pkg/v3/logutil",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/go.uber.org/zap:go_default_library",
        "//vendor/go.uber.org/zap/zapcore:go_default_library",
    ] + select({
        "@io_bazel_rules_go//go/platform:android": [
            "//vendor/github.com/coreos/go-systemd/v22/journal:go_default_library",
            "//vendor/go.etcd.io/etcd/client/pkg/v3/systemd:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:darwin": [
            "//vendor/github.com/coreos/go-systemd/v22/journal:go_default_library",
            "//vendor/go.etcd.io/etcd/client/pkg/v3/systemd:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:dragonfly": [
            "//vendor/github.com/coreos/go-systemd/v22/journal:go_default_library",
            "//vendor/go.etcd.io/etcd/client/pkg/v3/systemd:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:freebsd": [
            "//vendor/github.com/coreos/go-systemd/v22/journal:go_default_library",
            "//vendor/go.etcd.io/etcd/client/pkg/v3/systemd:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:ios": [
            "//vendor/github.com/coreos/go-systemd/v22/journal:go_default_library",
            "//vendor/go.etcd.io/etcd/client/pkg/v3/systemd:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:linux": [
            "//vendor/github.com/coreos/go-systemd/v22/journal:go_default_library",
            "//vendor/go.etcd.io/etcd/client/pkg/v3/systemd:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:nacl": [
            "//vendor/github.com/coreos/go-systemd/v22/journal:go_default_library",
            "//vendor/go.etcd.io/etcd/client/pkg/v3/systemd:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:netbsd": [
            "//vendor/github.com/coreos/go-systemd/v22/journal:go_default_library",
            "//vendor/go.etcd.io/etcd/client/pkg/v3/systemd:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:openbsd": [
            "//vendor/github.com/coreos/go-systemd/v22/journal:go_default_library",
            "//vendor/go.etcd.io/etcd/client/pkg/v3/systemd:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:plan9": [
            "//vendor/github.com/coreos/go-systemd/v22/journal:go_default_library",
            "//vendor/go.etcd.io/etcd/client/pkg/v3/systemd:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:solaris": [
            "//vendor/github.com/coreos/go-systemd/v22/journal:go_default_library",
            "//vendor/go.etcd.io/etcd/client/pkg/v3/systemd:go_default_library",
        ],
        "//conditions:default": [],
    }),
)
