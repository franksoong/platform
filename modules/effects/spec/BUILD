load("//tools:defaults.bzl", "jasmine_node_test", "ts_test_library")

ts_test_library(
    name = "test_lib",
    srcs = glob(
        [
            "**/*.ts",
        ],
        exclude = ["ngc/**/*.ts"],
    ),
    deps = [
        "//modules/effects",
        "//modules/store",
        "@npm//rxjs",
    ],
)

jasmine_node_test(
    name = "test",
    deps = [
        ":test_lib",
        "//modules/effects",
        "//modules/store",
    ],
)
