module = import('unstable-external_project')

# just a placeholder because the script name is required
project = module.add_project('configure',
    configure_options: [
        '--prefix=@PREFIX@',
        '--libdir=@LIBDIR@',
        '--incdir=@INCLUDEDIR@'
    ]
)

xputty_dep = project.dependency('xputty')
meson.override_dependency('xputty', xputty_dep, static: true)
