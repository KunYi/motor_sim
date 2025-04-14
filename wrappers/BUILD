package(default_visibility = ["//visibility:public"])

cc_library(
    name = "sdl2",
    copts = ["-I/usr/include/SDL2"],
    linkopts = ["-lSDL2"],
    visibility = ["//visibility:public"],
)

cc_library(
    name = "sdl_context",
    hdrs = ["sdl_context.h"],
    srcs = ["sdl_context.cpp"],
    copts = ["-I/usr/include/SDL2"],
    deps = [
        ":sdl2"
    ]
)
cc_library(
    name = "sdl_imgui",
    hdrs = ["sdl_imgui.h",
            "sdl_imgui_context.h"],
    srcs = ["sdl_imgui_context.cpp"],
    deps = [
        ":sdl2",
        "//third_party/imgui:imgui_sdl",
    ],
    copts = ["-I/usr/include/SDL2"]
)
