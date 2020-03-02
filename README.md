# script-CreateProject
Bash script to create a new C++ project folder.

## How to use
```$ CreateProject [Project]```

It would create a hello world cpp program with a CMakeLists.txt, which would be cmake-ed and make-ed to get a shared library and an exectuable in the following folder structure:

```
[Project]
├── build
│   ├── debug
│   └── release
│       ├── CMakeCache.txt
│       ├── CMakeFiles
│       ├── cmake_install.cmake
│       ├── compile_commands.json
│       ├── lib[Project].so
│       ├── Makefile
│       └── [Project]Test
├── CMakeLists.txt
└── code
    ├── include
    │   └── test.hpp
    └── src
        └── main.cpp

```

## Requirements
- CMake 3.0
