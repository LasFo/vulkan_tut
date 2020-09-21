load("@rules_cc//cc:defs.bzl", "cc_binary")

platform(
	name = "x64_windows-clang-cl",
	constraint_values = [
	  "@platforms//cpu:x86_64",
	  "@platforms//os:windows",
	  "@bazel_tools//tools/cpp:clang-cl",
	],
)

cc_binary(name = "main",
          srcs = ["main.cpp"],
          deps = ["//1.2.141.2/Include:vulkan", "@glfw//:glfw",],
          copts = ["-Xclang -std=c++17"],
          features = [ "fully_static_link" ],
          )

