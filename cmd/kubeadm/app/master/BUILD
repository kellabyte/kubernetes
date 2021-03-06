package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_binary",
    "go_library",
    "go_test",
    "cgo_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "addons.go",
        "apiclient.go",
        "discovery.go",
        "kubeconfig.go",
        "manifests.go",
        "pki.go",
        "tokens.go",
    ],
    tags = ["automanaged"],
    deps = [
        "//cmd/kubeadm/app/apis/kubeadm:go_default_library",
        "//cmd/kubeadm/app/apis/kubeadm/v1alpha1:go_default_library",
        "//cmd/kubeadm/app/images:go_default_library",
        "//cmd/kubeadm/app/util:go_default_library",
        "//pkg/api:go_default_library",
        "//pkg/api/errors:go_default_library",
        "//pkg/api/resource:go_default_library",
        "//pkg/api/v1:go_default_library",
        "//pkg/apis/extensions/v1beta1:go_default_library",
        "//pkg/apis/meta/v1:go_default_library",
        "//pkg/client/clientset_generated/release_1_5:go_default_library",
        "//pkg/client/unversioned/clientcmd:go_default_library",
        "//pkg/client/unversioned/clientcmd/api:go_default_library",
        "//pkg/kubectl/cmd/util:go_default_library",
        "//pkg/registry/core/service/ipallocator:go_default_library",
        "//pkg/util/cert:go_default_library",
        "//pkg/util/intstr:go_default_library",
        "//pkg/util/uuid:go_default_library",
        "//pkg/util/wait:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = [
        "addons_test.go",
        "apiclient_test.go",
        "discovery_test.go",
        "kubeconfig_test.go",
        "manifests_test.go",
        "pki_test.go",
        "tokens_test.go",
    ],
    library = "go_default_library",
    tags = ["automanaged"],
    deps = [
        "//cmd/kubeadm/app/apis/kubeadm:go_default_library",
        "//pkg/api/v1:go_default_library",
        "//pkg/util/cert:go_default_library",
        "//pkg/util/intstr:go_default_library",
    ],
)
