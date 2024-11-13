# bazel-root
Bazel monorepo root, to contain other repos.

Sets up bazel with the following dependencies

* Python 3.10
* Pybind11
* Google protobuf
* Pip
	- Numpy
	- Pygame
* hedron_compile_commands

Additionally, using the `hedron_compile_commands` we can generate
a compile_commands.json file for vscode.
`bazel run @hedron_compile_commands//:refresh_all`

Repositories are placed in subfolders to the root,
for example https://github.com/jonasnylund/gsim uses this setup.
