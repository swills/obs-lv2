project('obs-lv2', 'cpp', license : 'GPL2+')

deps =  [
  dependency('lv2', version : '>=1.16.0'),
  dependency('libobs'),
  dependency('lilv-0'),
  dependency('suil-0'),
  dependency('Qt5Widgets'),
]

sources = [
  'obs-lv2.cpp',
  'ui.cpp',
  'ui_timer.cpp',
  'urid.cpp',
  'state.cpp',
  'ports.cpp',
  'core.cpp',
]

shared_library(meson.project_name(),
	       sources,
	       dependencies : deps,
	       name_prefix : '',
	       install: true,
	       install_dir : get_option('libdir') / 'obs-plugins')
