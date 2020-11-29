# libigl example project

A blank project example showing how to use libigl and cmake. Feel free and
encouraged to copy or fork this project as a way of starting a new personal
project using libigl.

Because I had a few problems with CGAL, I changed the `CMakeLists` to use CGAL in the system path when Using `cmake`
(if you've already set up the CGAL system variables as described in the [tutorial](https://doc.cgal.org/latest/Manual/general_intro.html))

You can check the `CMakeLists` file to see what changes have been made

# Usage

## See the tutorial first

Then build, run and understand the [libigl tutorial](http://libigl.github.io/libigl/tutorial/).

## Dependencies

(**Maybe**) :sweat_smile: The only dependencies are stl, eigen, [libigl](http://libigl.github.io/libigl/) and
the dependencies of the `igl::opengl::glfw::Viewer`.

The cmake build system will attempt to find libigl according to environment variables (e.g., `LIBIGL`) and searching in common desitinations (e.g., `/usr/local/libigl/`). If you haven't installed libigl before, we recommend you to clone a copy of libigl right here:

    cd libigl-example-project/
    git clone https://github.com/libigl/libigl.git
    
## Compile

Compile this project using the standard cmake routine:

    mkdir build
    cd build
    cmake ..
    make
    
Or for Windows uesr:

    mkdir build
    cd build
    cmake-gui ..
    choose the corresponding VS version then configure and generate
    
If it goes well, we're basically done. Unfortunately, `cmake` might throw an error like this:

    Build step for Eigen failed: 1

GitLAB is not accessible in some regions due to network reasons, so I recommend you to clone `libigl` [here](https://github.com/broccoli-97/libigl)

A libigl repository with external




## Run

From within the `build` directory just issue:

    ./example or open example.sln with VS

A glfw app should launch displaying a 3D cube.
