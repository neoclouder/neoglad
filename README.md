# neoglad

This project stores [glad2](https://github.com/Dav1dde/glad/blob/glad2) OpenGL C/C++ headers only files to be easily used with CMkake.

Each OpenGL version (starting from 3.0) has a dedicated branch: `gl-<version>` (e.g. `gl-3.3`).

## Usage

In a CMake file:

    FetchContent_Declare(
        neoglad
        GIT_REPOSITORY https://github.com/neoclouder/neoglad.git
        GIT_TAG gl-3.3 # OpenGL version (git branch)
        GIT_SHALLOW	   TRUE
    )

    FetchContent_MakeAvailable(neoglad)
