py3.extension_module('_test_fortran',
  [
    f2py_gen.process('test_fortran.pyf'),
    '_test_fortran.f'
  ],
  c_args: [Wno_unused_variable],
  fortran_args: fortran_ignore_warnings,
  link_args: version_link_args,
  dependencies: [lapack_dep, fortranobject_dep],
  install: true,
  link_language: 'fortran',
  subdir: 'scipy/io',
  install_tag: 'tests'
)

py3.install_sources([
    '__init__.py',
    '_fortran.py',
    '_idl.py',
    '_mmio.py',
    '_netcdf.py',
    'harwell_boeing.py',
    'idl.py',
    'mmio.py',
    'netcdf.py',
    'wavfile.py'
  ],
  subdir: 'scipy/io'
)

subdir('tests')
subdir('matlab')
subdir('arff')
subdir('_harwell_boeing')
subdir('_fast_matrix_market')
