load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["storage_apiserver.go"],
    importpath = "k8s.io/kubernetes/pkg/registry/admissionregistration/rest",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/k8s.io/api/admissionregistration/v1alpha1:go_default_library",
        "//vendor/k8s.io/api/admissionregistration/v1beta1:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/registry/generic:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/registry/rest:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/server:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/server/storage:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/api/legacyscheme:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/admissionregistration:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/registry/admissionregistration/initializerconfiguration/storage:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/registry/admissionregistration/mutatingwebhookconfiguration/storage:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/registry/admissionregistration/validatingwebhookconfiguration/storage:go_default_library",
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
