load("//tools:build_rules/shims.bzl", "go_library", "go_test")

package(default_visibility = ["//kythe:default_visibility"])

go_library(
    name = "proxy",
    srcs = ["proxy.go"],
    deps = [
        "//kythe/proto:analysis_go_proto",
        "//kythe/proto:storage_go_proto",
    ],
)

go_test(
    name = "proxy_test",
    size = "small",
    srcs = ["proxy_test.go"],
    library = "proxy",
)
