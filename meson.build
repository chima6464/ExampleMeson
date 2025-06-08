project('Example Meson Project',
	'c',
	default_options : [
		'c_std=c11'
        
	],
	license: 'MIT',
	meson_version: '>=1.1.0',
	version: '1.0')

printf_subproject = subproject('printf')

libprintf_dep = printf_subproject.get_variable('libprintf_dep')
# Tell meson to navigate to subdirectory 
subdir('src')

