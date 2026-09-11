project('kibaos-welcome', 'vala', 'c')

# Dependencies
gtk_dep = dependency('gtk4')
adw_dep = dependency('libadwaita-1')
gio_dep = dependency('gio-2.0')

# Source files
sources = files(
    'main.vala'
)

# Executable
executable('kibaos-welcome', sources,
    dependencies: [gtk_dep, adw_dep, gio_dep],
    install: true
)

# Install desktop file
install_data(
    'welcome.desktop',
    install_dir: join_paths(get_option('datadir'), 'applications')
)

# Install CSS
css = import('data')
css.install_data(
    'welcome.css',
    install_dir: join_paths(get_option('datadir'), 'kibaos-welcome')
)
