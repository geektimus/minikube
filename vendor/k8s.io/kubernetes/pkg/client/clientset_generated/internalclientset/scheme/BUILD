package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "register.go",
        "register_custom.go",
    ],
    importpath = "k8s.io/kubernetes/pkg/client/clientset_generated/internalclientset/scheme",
    deps = [
        "//pkg/apis/admissionregistration/install:go_default_library",
        "//pkg/apis/apps/install:go_default_library",
        "//pkg/apis/authentication/install:go_default_library",
        "//pkg/apis/authorization/install:go_default_library",
        "//pkg/apis/autoscaling/install:go_default_library",
        "//pkg/apis/batch/install:go_default_library",
        "//pkg/apis/certificates/install:go_default_library",
        "//pkg/apis/componentconfig/install:go_default_library",
        "//pkg/apis/core/install:go_default_library",
        "//pkg/apis/events/install:go_default_library",
        "//pkg/apis/extensions/install:go_default_library",
        "//pkg/apis/networking/install:go_default_library",
        "//pkg/apis/policy/install:go_default_library",
        "//pkg/apis/rbac/install:go_default_library",
        "//pkg/apis/scheduling/install:go_default_library",
        "//pkg/apis/settings/install:go_default_library",
        "//pkg/apis/storage/install:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apimachinery/announced:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apimachinery/registered:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime/serializer:go_default_library",
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
