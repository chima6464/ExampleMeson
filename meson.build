project('Example Meson Project',
	'c',
	default_options : [
		'c_std=c11',
		'c_args=-Wall',
	],
	license: 'MIT',
	meson_version: '>=1.1.0',
	version: '1.0')

# Add source directories to the include path
inc = include_directories('include')
root_inc = include_directories('.')

printf_subproject = subproject('printf')

libprintf_dep = printf_subproject.get_variable('libprintf_dep')

openlibm_subproject = subproject('openlibm')
# Add the new openlibm dependency. Meson will use the .wrap file to find it.
openlibm_dep = openlibm_subproject.get_variable('openlibm_dep')

# Tell meson to navigate to subdirectory 
subdir('src')

