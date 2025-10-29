filesearch_sources = [
  'main.vala',
  'application.vala',
  'window.vala',
]

filesearch_deps = [
  config_dep,
  dependency('gtk4'),
  dependency('libadwaita-1', version: '>= 1.4'),
]

filesearch_sources += gnome.compile_resources('filesearch-resources',
  'filesearch.gresource.xml',
  c_name: 'filesearch'
)

executable('filesearch', filesearch_sources,
  dependencies: filesearch_deps,
  include_directories: config_inc,
       install: true,
)
