# Description:
#   Package groups for restricting access to config_feature_flag to specific
#   packages, allowing for careful rollout as it is an experimental feature.

filegroup(
    name = "srcs",
    srcs = glob(["**"]),
    visibility = ["//tools/whitelists:__pkg__"],
)

package_group(
    name = "config_feature_flag",
    includes = ["//tools/allowlists/config_feature_flag"],
)
