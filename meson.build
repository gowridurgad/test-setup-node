project('pygobject-sample', 'c', 'python',
  version: '0.1.0',
  default_options: ['warning_level=3'])

pygobject_dep = dependency('pygobject-3.0', version: '>= 3.40.1')

py3_mod = import('python')
py3 = py3_mod.find_installation('python3')

py3.extension_module('example',
  sources: 'example.c',
  dependencies: pygobject_dep,
  install: true)
