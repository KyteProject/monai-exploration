# monai-exploration

MONAI Deploy App SDK’s core functionality is written in Python 3 (>= 3.8) for
Linux.

`pip install monai-deploy-app-sdk`

If you have installed MONAI Deploy App SDK previously, you can upgrade to the
latest version with:

`pip install --upgrade monai-deploy-app-sdk`

For packaging your application, MONAI Application Packager and MONAI Application
Runner (MAR) requires NVIDIA Docker (NVIDIA Container Toolkit) installed:

https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html#docker

Currently, `nvcr.io/nvidia/clara-holoscan/holoscan:v0.6.0-dgpu` base Docker
image is used by MONAI Application Packager by default for X86-64 in Linux
system.

The base image size is large so please pull the image in advance to save time.
Note that the container image tag in the following example, e.g. v0.6.0,
corresponds to the SDK version.

`docker pull nvcr.io/nvidia/clara-holoscan/holoscan:v0.6.0-dgpu`

Windows users can install CUDA on WSL to use MONAI Deploy App SDK.
