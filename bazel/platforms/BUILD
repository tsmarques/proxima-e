constraint_setting(name = "mcu")

constraint_value(
    name = "mcu_cortex_m4",
    constraint_setting = ":mcu",
    visibility = ["//visibility:public"],
)

platform(
    name = "cortex_m4",
    constraint_values = [
        "@platforms//cpu:armv7e-m",
        "@platforms//os:none",
        ":mcu_cortex_m4",
    ],
    visibility = ["//visibility:public"],
)
