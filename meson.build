cherrrb_src = files('chry_ringbuffer.c')

cherrrb_dep = declare_dependency(
  sources: cherrrb_src,
  include_directories: include_directories('.'),
)

meson.override_dependency('CherryRB', cherrrb_dep)
