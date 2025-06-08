#This build file intelligently handles the different architectures by setting the correct include paths based on the host machine. It then declares a system dependency, 
#which can be used by the rest of your project.

project('openlibm-patch', 'c')

# Detect host architecture and set include path accordingly
host_arch = host_machine.cpu_family()
openlibm_arch_dir = ''
if host_arch == 'x86_64'
  # The specified commit has i387 headers for the x86 family.
  openlibm_arch_dir = 'src/i387'
elif host_arch == 'aarch64'
  openlibm_arch_dir = 'src/aarch64'
elif host_arch == 'arm'
  openlibm_arch_dir = 'src/arm'
else
  # Add other architectures if needed, for now we will error out.
  error('Unsupported architecture for openlibm: ' + host_arch)
endif

# Create a list of include directories, marking them as system headers
openlibm_inc = include_directories(
    'include',
    'src',
    openlibm_arch_dir,
    is_system: true
)

# Declare the dependency for the parent project to use
openlibm_dep = declare_dependency(
    include_directories: openlibm_inc,
)

# Override the 'openlibm' dependency to provide our declared dependency
meson.override_dependency('openlibm', openlibm_dep)