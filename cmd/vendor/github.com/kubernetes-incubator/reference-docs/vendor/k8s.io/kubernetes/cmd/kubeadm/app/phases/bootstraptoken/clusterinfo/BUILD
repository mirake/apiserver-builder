package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_test(
    name = "go_default_test",
    srcs = ["clusterinfo_test.go"],
    importpath = "k8s.io/kubernetes/cmd/kubeadm/app/phases/bootstraptoken/clusterinfo",
    library = ":go_default_library",
    deps = [
        "//vendor/k8s.io/apimachinery/pkg/api/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes/fake:go_default_library",
        "//vendor/k8s.io/client-go/testing:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/api:go_default_library",
    ],
)

go_library(
    name = "go_default_library",
    srcs = ["clusterinfo.go"],
    importpath = "k8s.io/kubernetes/cmd/kubeadm/app/phases/bootstraptoken/clusterinfo",
    deps = [
        "//vendor/k8s.io/api/core/v1:go_default_library",
        "//vendor/k8s.io/api/rbac/v1beta1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/user:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes:go_default_library",
        "//vendor/k8s.io/client-go/tools/clientcmd:go_default_library",
        "//vendor/k8s.io/client-go/tools/clientcmd/api:go_default_library",
        "//vendor/k8s.io/kubernetes/cmd/kubeadm/app/util/apiclient:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/rbac/v1beta1:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/bootstrap/api:go_default_library",
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
)
