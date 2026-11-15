load("@arm_none_eabi//toolchain:toolchain.bzl", "arm_none_eabi_toolchain")

arm_none_eabi_toolchain(
    name = "cortex_m4_toolchain",
    copts = [
        "-mcpu=cortex-m4",
        "-mthumb",
        "-fno-canonical-system-headers",
        "-no-canonical-prefixes",
        "-nostdinc",
        "-Og",
        "-Wall",
        "-fdata-sections",
        "-ffunction-sections",
        "-MMD",
        "-MP",
        "-std=c++17",
        "-fno-rtti",
        "-fno-exceptions",
    ],
    linkopts = [
        "-mcpu=cortex-m4",
        "-mthumb",
        "--specs=nosys.specs",
        "-specs=nano.specs",
        "-lc",
        "-lm",
        "-lnosys",
        "-lstdc++",
    ],
    target_compatible_with = [
        "@platforms//cpu:armv7e-m",
        "@platforms//os:none",
        "//bazel/platforms:mcu_cortex_m4",
    ],
)
