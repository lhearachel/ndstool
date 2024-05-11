project('nds-tool', 'c', 'cpp', version: '2.2.0')

subdir('source')

public_includes = include_directories('source')

ndstool_exe = executable('ndstool',
    sources: cpp_sources,
    cpp_args: [
        '-DPACKAGE_NAME="ndstool"',
        '-DPACKAGE_TARNAME="ndstool"',
        '-DPACKAGE_VERSION="2.2.0"',
        '-DPACKAGE_STRING="ndstool\ 2.2.0"',
        '-DPACKAGE_BUGREPORT="https://github.com/devkitPro/ndstool/issues"',
        '-DPACKAGE_URL=""',
        '-DPACKAGE="ndstool"',
        '-DVERSION="2.2.0"',
    ],
    include_directories: public_includes,
    build_by_default: true,
)

meson.override_find_program('ndstool', ndstool_exe)
