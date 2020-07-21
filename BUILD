load("@rules_java//java:defs.bzl", "java_binary", "java_library", "java_test")

java_library(
    name = "target",
    srcs = ["target/Target.java"],
)

java_library(
    name = "reference",
    srcs = ["reference/Reference.java"],
    deps = [":target"],
)

java_test(
    name = "target_test",
    srcs = ["target/TargetTest.java"],
    deps = [":target"],
    test_class = "example.TargetTest",
)

java_test(
    name = "reference_test",
    srcs = ["reference/ReferenceTest.java"],
    deps = [":reference"],
    test_class = "example.ReferenceTest",
)