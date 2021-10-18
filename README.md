# i_robot
Small collection of models and example programs illustrating robotics visualization using VulkanSceneGraph.

## Dependencies

* [VulkanSDK]() - VulkanSDK 1.2.162.0 or later
* [VulkanSceneGraph](https://github.com/vsg-dev/VulkanSceneGraph) - VulaknSceneGraph-0.1.7 or later
* [CMake](https://cmake.org) - cmake-3.7 or later.
* C++17 or later compiler

# Optional dependencies
* [vsgXchange](https://github.com/vsg-dev/vsgXchange)_- optional vsgXchange-0.0.0 or later
* [vsgImGui](https://github.com/vsg-dev/vsgImGui)_- optional vsgImGui-0.0.0 or later

# Building i_robot

Unix in source build:

    cd i_robot
    cmake .
    make -j 8

All examples applications and placed in i_robot/bin when built, and will be installed in standard sysmtem directories. Install path can be manually set via the standard CMAKE_INSTALL_PREFIX variable.

To install:

    make install

To execuate the examples with run directly from the local bin by or by setting the PATH env variable to the i_robot/bin directory, or running install.

## Robot models

The following robot models are from bullet3's [examples/pybullet/gym/pybullet_data](https://github.com/bulletphysics/bullet3/tree/master/examples/pybullet/gym/pybullet_data) collection of .urdf models, converted from urdf to vsgt (VulkanSceneGraph ascii format):

* [data/robots/a1.vsgt](data/robots/a1.vsgt)
* [data/robots/mini_cheetah.vsgt](data/robots/mini_cheetah.vsgt)
* [data/robots/racecar.vsgt](data/robots/racecar.vsgt)

## Terrain/environment models

The following models are originally from [vsgExamples](https://github.com/vsg-dev/vsgExamples)

* [data/models/lz.vsgt](data/models/lz.vsgt) - Ed Levin Park
* data/models/skybox.vsgb - sky environment model
