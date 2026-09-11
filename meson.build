project('kibaos-welcome', 'vala', 'c')

gtk_dep = dependency('gtk4')
adw_dep = dependency('libadwaita-1')
gio_dep = dependency('gio-2.0')

sources = files(
    'main.vala'
)

executable(
    'kibaos-welcome',
    sources,
    dependencies: [gtk_dep, adw_dep, gio_dep],
    install: true
)

install_data(
    'welcome.desktop',
    install_dir: join_paths(get_option('datadir'), 'applications')
)

install_data(
    'welcome.css',
    install_dir: join_paths(get_option('datadir'), 'kibaos-welcome')
)
