# Examples to build C++ code

This package will showcase how to build C++ code in stages.

### Stage 1
The first stage is really simple and shows you how to compile a binary with a single source file.

### Stage 2
The second stage will showcase how to build an application with multiple source and header files, separated in a library and a binary.

### Stage 3
The third stage showcases how to link multiple build directories by building multiple libraries in different packages and then connecting it up with the main application.

==============================================================================================================================================================
Bazel is an artifact based build system.
In this system, developers define the task but bazel defines how those tasks will be built. This means our targets are written in a declarative manner.

By analyzing all the components of a build, bazel can optimize the process.
E.g -> If nothing was previously changed, bazel will not rebuild it.
    -> If there isn't a dependency from previous tasks, bazel will run build targets in parallel.

=====================================================================================================================================================
Bazel Files:
1) WORKSPACE : Its just a simple text file that sits at the top level directory of project.
               It allows us to incorporate custom rules into our project as well as declare any dependencies that any build within the workspace may use
               Note: it can be empty they dont have to contain anything.

2) BUILD File : Here we will write our actual build instructions and define our targets
