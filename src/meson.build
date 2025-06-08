#NOTE: One benefit of using files() instead of just providing a list of files to the target (e.g., static_library) is that Meson handles the absolute location files for us with the files()interface. This means we can declare a files object in one directory and use it in another, 
#without any fear of adjusting the paths. 
#We prefer using files() by default because it makes for easier refactoring at a later date.

#Grouping files into "modules" for organization and future ability to include/exclude enitre files based on library configuration
gdtoa_files = files(
	'gdtoa/src/dmisc.c',
	'gdtoa/src/dtoa.c',
	'gdtoa/src/g__fmt.c',
	'gdtoa/src/g_ddfmt.c',
	'gdtoa/src/g_dfmt.c',
	'gdtoa/src/g_ffmt.c',
	'gdtoa/src/g_Qfmt.c',
	'gdtoa/src/g_xfmt.c',
	'gdtoa/src/g_xLfmt.c',
	'gdtoa/src/gdtoa.c',
	'gdtoa/src/gethex.c',
	'gdtoa/src/gmisc.c',
	'gdtoa/src/hd_init.c',
	'gdtoa/src/hexnan.c',
	'gdtoa/src/misc.c',
	'gdtoa/src/smisc.c',
	'gdtoa/src/strtod.c',
	'gdtoa/src/strtodg.c',
	'gdtoa/src/strtodI.c',
	'gdtoa/src/strtof.c',
	'gdtoa/src/strtoId.c',
	'gdtoa/src/strtoIdd.c',
	'gdtoa/src/strtoIf.c',
	'gdtoa/src/strtoIg.c',
	'gdtoa/src/strtoIQ.c',
	'gdtoa/src/strtoIx.c',
	'gdtoa/src/strtoIxL.c',
	'gdtoa/src/strtopd.c',
	'gdtoa/src/strtopdd.c',
	'gdtoa/src/strtopf.c',
	'gdtoa/src/strtopQ.c',
	'gdtoa/src/strtopx.c',
	'gdtoa/src/strtopxL.c',
	'gdtoa/src/strtord.c',
	'gdtoa/src/strtordd.c',
	'gdtoa/src/strtorf.c',
	'gdtoa/src/strtorQ.c',
	'gdtoa/src/strtorx.c',
	'gdtoa/src/strtorxL.c',
	'gdtoa/src/sum.c',
	'gdtoa/src/ulp.c'
)

assert_files = files('assert/assert.c')

crt_files = files(
	'crt/_Exit.c',
	'crt/abort.c',
	'crt/at_exit.c',
	'crt/at_quick_exit.c',
	'crt/crt.c',
	'crt/cxa_atexit.c',
	'crt/exit.c',
	'crt/quick_exit.c',
)

ctype_files = files(
	'ctype/isalnum.c',
	'ctype/isalpha.c',
	'ctype/isascii.c',
	'ctype/isblank.c',
	'ctype/iscntrl.c',
	'ctype/isdigit.c',
	'ctype/isgraph.c',
	'ctype/islower.c',
	'ctype/isprint.c',
	'ctype/ispunct.c',
	'ctype/isspace.c',
	'ctype/isupper.c',
	'ctype/isxdigit.c',
	'ctype/toascii.c',
	'ctype/tolower.c',
	'ctype/toupper.c'
)

stdlib_files = files(
	'stdlib/abs.c',
	'stdlib/atof.c',
	'stdlib/atoi.c',
	'stdlib/atol.c',
	'stdlib/atoll.c',
	'stdlib/bsearch.c',
	'stdlib/calloc.c',
	'stdlib/div.c',
	'stdlib/heapsort_r.c',
	'stdlib/heapsort.c',
	'stdlib/imaxabs.c',
	'stdlib/imaxdiv.c',
	'stdlib/labs.c',
	'stdlib/ldiv.c',
	'stdlib/llabs.c',
	'stdlib/lldiv.c',
	'stdlib/qsort_r.c',
	'stdlib/qsort.c',
	'stdlib/rand.c',
	'stdlib/realloc.c',
	'stdlib/strtol.c',
	'stdlib/strtold.c',
	'stdlib/strtoul.c',
	'stdlib/strtoll.c',
	'stdlib/strtoull.c',
)

wchar_files = files(
	'wchar/iswalnum.c',
	'wchar/iswalpha.c',
	'wchar/iswblank.c',
	'wchar/iswcntrl.c',
	'wchar/iswalnum.c',
	'wchar/iswalpha.c',
	'wchar/iswblank.c',
	'wchar/iswcntrl.c',
	'wchar/iswctype.c',
	'wchar/iswdigit.c',
	'wchar/iswgraph.c',
	'wchar/iswlower.c',
	'wchar/iswprint.c',
	'wchar/iswpunct.c',
	'wchar/iswspace.c',
	'wchar/iswupper.c',
	'wchar/iswxdigit.c',
	'wchar/towccase.c',
	'wchar/towctrans.c',
	'wchar/towlower.c',
	'wchar/towupper.c',
	'wchar/wcswidth.c',
	'wchar/wctrans.c',
	'wchar/wctype.c',
	'wchar/wcwidth.c',
)

locale_files = files(
	'locale/langinfo.c',
)

math_files = files(
	'math/fabs.c',
	'math/fabsf.c',
)

stdio_files = files(
	'stdio/asprintf.c',
	'stdio/putchar.c',
	'stdio/puts.c',
	'stdio/vasprintf.c',
)

support_files = files(
	'support/fls.c',
	'support/flsl.c',
	'support/flsll.c',
)

time_files = files(
	'time/asctime.c',
	'time/asctime_r.c',
)

string_files = files(
'string/memcmp.c',
'string/memcpy.c',
'string/memmem.c',
'string/memmove.c',
'string/memchr.c',
'string/memrchr.c',
'string/memset.c',
'string/strcat.c',
'string/strchr.c',
'string/strchrnul.c',
'string/strcmp.c',
'string/strcoll.c',
'string/strcpy.c',
'string/strcspn.c',
'string/strdup.c',
'string/strerror.c',
'string/strerror_r.c',
'string/strlen.c',
'string/strncat.c',
'string/strncmp.c',
'string/strncpy.c',
'string/strndup.c',
'string/strnlen.c',
'string/strnstr.c',
'string/strpbrk.c',
'string/strrchr.c',
'string/strspn.c',
'string/strstr.c',
'string/strtok.c',
'string/strxfrm.c',
)

#Ability to group files used by all libc targets 
libc_common_files = [
	assert_files,
	ctype_files,
	locale_files,
	math_files,
	stdio_files,
	stdlib_files,
	string_files,
	support_files,
	time_files,
	wchar_files,
]

# These files are used to compile libc for a build machine / your personal computer
libc_native_files = files(
	'stdio/putchar_native.c',
)

# These files are used when cross-compiling libc for another platform
libc_standalone_files = [
	crt_files,
]


#Like w/ gdtoa, also need an include_directories object that points to the proper header location for the C library headers. In this case, it is the top-level include directory. We’ll specify a relative path, 
#and the include_directories API will handle the proper conversion to the absolute path on our file system under the hood.
#The include directory could technically be the same directory as the src files as long as they exist there, but its much better to separate them
#for clarity

libc_includes = include_directories('../include')

gdtoa_includes = include_directories('gdtoa/include')

gdtoa_compiler_flags = [
	'-DNO_ERRNO',
	'-DIFNAN_CHECK',
	'-DGDTOA_NO_ASSERT',
	'-DNO_FENV_H',
	'-DNO_IEEE_Scale'
]


libgdtoa = static_library('gdtoa',
    gdtoa_files,
    include_directories: gdtoa_includes,
	c_args: gdtoa_compiler_flags, # New Addition
)


#To address include errors, you need to simply use include_directories to include the directory that possesses the header file.
arch_specific_includes = include_directories('../arch/x86_64/include')

libprintf_dep = printf_subproject.get_variable('libprintf_dep')

libc_native = static_library('c_native',
  libc_common_files + libc_native_files,
  include_directories: [libc_includes, arch_specific_includes],
  dependencies: libprintf_dep,
)

