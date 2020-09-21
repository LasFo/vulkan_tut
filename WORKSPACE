load("@bazel_tools//tools/build_defs/repo:git.bzl", "new_git_repository")

register_execution_platforms(
      ":x64_windows-clang-cl"
)

register_toolchains(
      "@local_config_cc//:cc-toolchain-x64_windows-clang-cl",
)

new_git_repository(
    name = "glm",
    remote = "https://github.com/g-truc/glm.git",
    commit = "23e0701c0483283440d4d1bcd17eb7070fa8eb75",
    build_file = "glm.BUILD",
)

new_git_repository(
    name = "glfw",
    remote = "https://github.com/glfw/glfw.git",
    commit = "8d7e5cdb49a1a5247df612157ecffdd8e68923d2",
    build_file = "glfw.BUILD",
)
