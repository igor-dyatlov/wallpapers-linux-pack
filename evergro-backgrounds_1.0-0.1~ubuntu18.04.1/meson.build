project('evergro-backgrounds',
  version: '1.0',
  license: [
    'GPL-2.0',
    'CC-BY-SA-4.0'
  ],
  meson_version: '>= 0.40.0'
)

# Dependencies
dep_glib = dependency('glib-2.0', version: '>= 2.48.0')

# Global paths
prefix = get_option('prefix')
datadir = join_paths(prefix, get_option('datadir'))
backgrounddir = join_paths(datadir, 'backgrounds', 'evergro')
metadatadir_gnome = join_paths(datadir, 'gnome-background-properties')
metadatadir_cinnamon = join_paths(datadir, 'cinnamon-background-properties')
metadatadir_mate = join_paths(datadir, 'mate-background-properties')

# Sub directories
subdir('backgrounds')

# Extra-dist files
extra_dist = [
  'AUTHORS'
]

install_data(extra_dist, install_dir: backgrounddir)
