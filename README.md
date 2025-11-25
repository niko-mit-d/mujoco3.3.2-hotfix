This repository fixes an issue present when installing MuJoCo on Windows, see [here](https://github.com/google-deepmind/mujoco/issues/2927). As the changes were only officially implemented on the latest version (as of November 2025), this repository implements the bug fix into version 3.3.2 of MuJoCo.

Run this to build and install the package:
```
mkdir build 
cd build
mkdir install_dir
cmake -DCMAKE_INSTALL_PREFIX=install_dir ..
cmake --build . --config RELEASE
cmake --install .
```
and add `install_dir/bin` to environment variables.