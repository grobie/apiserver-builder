package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_test",
)

go_test(
    name = "go_default_test",
    size = "large",
    srcs = [
        "defaulttolerationseconds_test.go",
        "main_test.go",
    ],
    importpath = "k8s.io/kubernetes/test/integration/defaulttolerationseconds",
    tags = [
        "etcd",
        "integration",
    ],
    deps = [
        "//vendor/k8s.io/api/core/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes:go_default_library",
        "//vendor/k8s.io/client-go/rest:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/api/helper:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/api/testapi:go_default_library",
        "//vendor/k8s.io/kubernetes/plugin/pkg/admission/defaulttolerationseconds:go_default_library",
        "//vendor/k8s.io/kubernetes/plugin/pkg/scheduler/algorithm:go_default_library",
        "//vendor/k8s.io/kubernetes/test/integration/framework:go_default_library",
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
