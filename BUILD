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
          deps = ["@bazel_tools//tools/cpp/runfiles", "//1.2.141.2/Include:vulkan", "@glfw//:glfw",],
          data = ["shaders/frag.spv", "shaders/vert.spv"],
          copts = ["-Xclang -std=c++17"],
          features = [ "fully_static_link" ],
          )

