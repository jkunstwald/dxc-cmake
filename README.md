# DXC CMake

Get DXC to build in a CMake context. This should work right away, but note:

## Windows

DXC requires TAEF, make sure that the [Windows Driver Kit](https://docs.microsoft.com/en-us/windows-hardware/drivers/download-the-wdk) is installed.

## Linux

The build directory must not contain spaces, as some tool invocations in DXCs build process incorrectly escape them.
