package(default_visibility = ["//visibility:public"])

load("@org_tensorflow_tensorboard//tensorboard/defs:web.bzl", "tf_web_library")

licenses(["notice"])  # Apache 2.0

tf_web_library(
    name = "facets_overview_chart",
    srcs = [
        "facets-overview-chart.html",
        "facets-overview-chart.ts"
    ],
    clutz_entry_points = [
        "proto.featureStatistics.DatasetFeatureStatistics",
        "proto.featureStatistics.DatasetFeatureStatisticsList",
        "proto.featureStatistics.FeatureNameStatistics",
        "proto.featureStatistics.NumericStatistics",
        "proto.featureStatistics.StringStatistics",
        "proto.featureStatistics.CommonStatistics",
        "proto.featureStatistics.Histogram",
        "proto.featureStatistics.RankHistogram"
    ],
    path = "/facets-overview/components/facets-overview-chart",
    deps = [
        "//facets_overview/proto",
        "//facets_overview/common",
        "@org_polymer_iron_list",
        "@org_polymer_paper_button",
        "@org_polymer_paper_checkbox",
        "@org_tensorflow_tensorboard//tensorboard/components/tf_imports:d3",
        "@org_tensorflow_tensorboard//tensorboard/components/tf_imports:plottable",
        "@org_tensorflow_tensorboard//tensorboard/components/tf_imports:polymer",
    ],
)
