project('fastgltf', 'cpp', version: '1.0.0')

fastgltf_src = []

subdir('src')

fastgltf_deps = []

fastgltf_include = [
    include_directories('include')
]

fastgltf = library(
    'fastgltf',
    fastgltf_src,
    include_directories: fastgltf_include,
    install: true
)

fastgltf_dep = declare_dependency(
    link_with: fastgltf,
    include_directories: fastgltf_include,
    dependencies: fastgltf_deps
)
