libmutk_sources = files([
  'version.cpp',
  'call.cpp',
  'pedigree.cpp',
  'utility.cpp',
  'newick.cpp',
  'relationship_graph.cpp',
  'mutation.cpp'
])

libmutk_deps = [boost_dep, doctest_dep, eigen_dep]

libmutk = static_library('mutk', [libmutk_sources, version_file],
  include_directories : inc,
  dependencies : libmutk_deps,
  cpp_args : ['-DDOCTEST_CONFIG_DISABLE']
)
