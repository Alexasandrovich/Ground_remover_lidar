# Ground segmentation method for 3D LiDAR scans (baseline - https://github.com/url-kaist/patchwork-plusplus)

## :package: Prerequisite packages
> You may need to install Eigen, numpy, and Open3D. Open3D is used for point cloud visualization.

```bash
# To install Eigen and numpy
$ sudo apt-get install libeigen3-dev
$ pip install numpy

# To install Open3D Python packages
$ pip install open3d

# To install Open3D C++ packages
$ git clone https://github.com/isl-org/Open3D
$ cd Open3D
$ util/install_deps_ubuntu.sh # Only needed for Ubuntu
$ mkdir build && cd build
$ cmake ..
$ make
$ sudo make install
```

## :gear: How to build
> Please follow below codes to build Patchwork++.

```bash
$ git clone https://github.com/url-kaist/patchwork-plusplus
$ cd patchwork-plusplus
$ mkdir build && cd build
$ cmake ..
$ make
```

## :runner: To run the demo codes

### C++
```bash

# Run with your point cloud file (pcd/SemanticKitti), example here
$ ./build/examples/cpp/demo_visualize ./data/000000.bin
$ ./build/examples/cpp/demo_visualize ./data/vlp_32_c/test.pcd

```