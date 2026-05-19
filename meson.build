project(
    'wxwidget-test',
    'cpp',
    version: '1.0.14',
    default_options: ['cpp_std=c++20'],
)

cmake = import('cmake')
sub_proj = cmake.subproject('wxWidgets')
message('CMake targets:\n - ' + '\n - '.join(sub_proj.target_list()))
wxwidgets_dep = sub_proj.dependency('wxWidgets')
dependencies = [wxwidgets_dep]

a = executable('a', files('a.cpp'), dependencies: dependencies)
