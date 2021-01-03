# add_cuda_path

Script to add CUDA PATH variables directories at the system level.

The profile script allows CUDA environment variables to be enabled for all users.

Tested on Ubuntu 18.04, but should work on other Linux instances.

## Installation
It's recommended to create a symbolic link from the desired CUDA directory to /usr/local/cuda.

Example:
> ln -sf /usr/local/cuda-10.2 /usr/local/cuda

The script looks for a CUDA installation under /usr/local/cuda

For multiple CUDA installations, simply update the symbolic link to point towards the desired CUDA version.

Copy the shell script to /etc/profile.d/ as root

> sudo cp cuda.sh /etc/profile.d/
