# CMake Project Template

This template is a starting point for a CMake-based project, including some formatting rules that are customized to my coding style


## Project Structure
This project follows the [Pitchfork Layout](https://api.csswg.org/bikeshed/?force=1&url=https://raw.githubusercontent.com/vector-of-bool/pitchfork/develop/data/spec.bs) for C++ projects. Specifically:
- `src`: Source files and the private headers.
- `build`: Build artifacts. (Not part of the repo.)
- `data`: Non-source files, like INI files.
- `docs`: Documentation.
- `examples`: Samples and the examples.
- `external`: Used external projects.
- `extras`: Submodules not build by default.
- `include`: Public headers.
- `libs`: Submodules build by default.
- `tests`: Tests cases.
- `tools`: Development utilities.

This allows easy integration with CMake using `add_subdirectory`, also allowing conditionally builds like not building the test suite

## Usage
To use the project, simply clone the repository and configure the following:
- `CMakeLists.txt` - change the name of the project to your project name
- `.vscode/launch.json` - change the name of the project to your project name