package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_library(
    name = "go_default_library",
    srcs = ["admission.go"],
    tags = ["automanaged"],
    deps = [
        "//vendor/k8s.io/apimachinery/pkg/api/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/labels:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/admission:go_default_library",
        "//vendor/k8s.io/sample-apiserver/pkg/admission/wardleinitializer:go_default_library",
        "//vendor/k8s.io/sample-apiserver/pkg/apis/wardle:go_default_library",
        "//vendor/k8s.io/sample-apiserver/pkg/client/informers_generated/internalversion:go_default_library",
        "//vendor/k8s.io/sample-apiserver/pkg/client/listers_generated/wardle/internalversion:go_default_library",
    ],
)

go_test(
    name = "go_default_xtest",
    srcs = ["admission_test.go"],
    tags = ["automanaged"],
    deps = [
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/admission:go_default_library",
        "//vendor/k8s.io/client-go/testing:go_default_library",
        "//vendor/k8s.io/sample-apiserver/pkg/admission/plugin/banflunder:go_default_library",
        "//vendor/k8s.io/sample-apiserver/pkg/admission/wardleinitializer:go_default_library",
        "//vendor/k8s.io/sample-apiserver/pkg/apis/wardle:go_default_library",
        "//vendor/k8s.io/sample-apiserver/pkg/client/clientset_generated/internalclientset/fake:go_default_library",
        "//vendor/k8s.io/sample-apiserver/pkg/client/informers_generated/internalversion:go_default_library",
    ],
)
