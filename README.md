# odin-unreal-tutorial
Project accompanying the unreal tutorial.

## Getting Started

Clone the git repo into a working directory of your choice.

This repository uses [LFS](https://git-lfs.github.com) (large file storage) to manage pre-compiled binaries. Note that a standard clone of the repository might only retrieve the metadata about these files managed with LFS. In order to retrieve the actual data with LFS, please follow these steps:

1. Clone the repository:  
   ```
   git clone https://github.com/4Players/odin-unreal-tutorial.git
   ```

2. Cache the actual LFS data on your local machine and replace the metadata in the binary files with their actual contents: 
   ```
   git lfs fetch
   git lfs checkout
   ```
   ... or if you have a recent LFS version:
   ```
   git lfs pull
   ```

### Installing Visual Studio and Compiling the Project

Sometimes it is necessary to compile from Visual Studio:

1. Download the newest version of Visual Studio: https://visualstudio.microsoft.com/de/
2. Community Edition is fine for this project.
3. Open the installer.
4. Make sure to enable "Game development withC++" Workload. And then include "Unreal Engine installer" and "Windows 10 SDK" in its options on the right side of the Installer's Window.
5. You might need to right-click the `OdinUnrealSample.uproject` file and `Generate Visual Studio project files`.
6. Double-click the `OdinUnrealSample.uproject`
7. It should compile automatically now. If this does not work, open the `OdinUnrealSample.sln` file instead.
8. Visual Studio will open.
9. Once done hit F5 to start the debugger - and compile using Visual Studio.
