package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "callback.go",
        "http.go",
        "push.go",
        "report.go",
        "setting.go",
    ],
    importpath = "go-common/app/interface/main/push/http",
    tags = ["automanaged"],
    deps = [
        "//app/interface/main/push/conf:go_default_library",
        "//app/interface/main/push/service:go_default_library",
        "//app/service/main/push/dao/huawei:go_default_library",
        "//app/service/main/push/dao/jpush:go_default_library",
        "//app/service/main/push/dao/mi:go_default_library",
        "//app/service/main/push/dao/oppo:go_default_library",
        "//app/service/main/push/model:go_default_library",
        "//library/ecode:go_default_library",
        "//library/log:go_default_library",
        "//library/net/http/blademaster:go_default_library",
        "//library/net/http/blademaster/middleware/auth:go_default_library",
        "//library/time:go_default_library",
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
