# DXC CMake

Get DXC to build in a CMake context. This should work right away, but note:

## Windows

DXC requires that the [Windows Driver Kit (WDK)](https://docs.microsoft.com/en-us/windows-hardware/drivers/download-the-wdk) is installed for the active Windows 10 SDK version.

If compilation fails because `#include "D3D12TokenizedProgramFormat.hpp"` does not resolve, the WDK is likely missing. This file is searched for in `C:\Program Files (x86)\Windows Kits\10\Include\<SDK VERSION>\um\`.

## Linux

The build directory must not contain spaces, as some tool invocations in DXCs build process incorrectly escape them.
