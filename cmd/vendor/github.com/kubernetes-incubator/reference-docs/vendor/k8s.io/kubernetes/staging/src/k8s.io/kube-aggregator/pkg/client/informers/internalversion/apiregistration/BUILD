package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["interface.go"],
    importpath = "k8s.io/kubernetes/staging/src/k8s.io/kube-aggregator/pkg/client/informers/internalversion/apiregistration",
    deps = [
        "//vendor/k8s.io/kube-aggregator/pkg/client/informers/internalversion/apiregistration/internalversion:go_default_library",
        "//vendor/k8s.io/kube-aggregator/pkg/client/informers/internalversion/internalinterfaces:go_default_library",
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
    srcs = [
        ":package-srcs",
        "//staging/src/k8s.io/kube-aggregator/pkg/client/informers/internalversion/apiregistration/internalversion:all-srcs",
    ],
    tags = ["automanaged"],
)
