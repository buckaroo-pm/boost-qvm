load('//:buckaroo_macros.bzl', 'buckaroo_deps')
load('//:subdir_glob.bzl', 'subdir_glob')

prebuilt_cxx_library(
  name = 'qvm',
  header_only = True,
  header_namespace = 'boost',
  exported_headers = subdir_glob([
    ('include/boost', '**/*.hpp'),
  ]),
  deps = buckaroo_deps(),
  visibility = [
    'PUBLIC',
  ],
)
