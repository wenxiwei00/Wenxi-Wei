# Wenxi-Wei
Lab 2

# Content
* Arm GNU Toolchain
* CMake
* Build Tools for Visual Studio 2022
* Python 3.10
* Git
* Getting the SDK and examples
* Building "Hello World"
* Putty

# Arm GNU Toolchain
Download Arm GNU Toolchain from https://developer.arm.com/downloads/-/arm-gnu-toolchain-downloads. Choose the highlighted version.

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/1.1.PNG" width="600px">

Tick all boxes in this step.

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/1.3.PNG" width="500px">

# CMake
Download CMake from https://cmake.org/download/. Choose the highlighted version.

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/2.1.PNG" width="500px">

Do not forget to choose "Add CMake to the system PATH for all users"

# Build Tools for Visual Studio 2022
Download from https://visualstudio.microsoft.com/zh-hans/downloads/.

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/3.1.PNG" width="500px">

# Python 3.10
Download from https://www.python.org/downloads/windows/.
hhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhhh 4.1

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/1.3.PNG" width="500px">

# Git
Download from https://git-scm.com/download/win.
5.15555555555555555555555555555555555

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/1.3.PNG" width="500px">

# Getting the SDK and examples
Open Visual Studio Code >> Terminal >> New Terminal.
Initial the address
```
PS D:\app\519\pico\pico-examples> cd "D:\app\519\pico"
```
6.11111111111
<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/1.3.PNG" width="500px">

Then, clone SDK and example from github
```
PS D:\app\519\pico> git clone -b master https://github.com/raspberrypi/pico-sdk.git  
PS D:\app\519\pico> cd pico-sdk
PS D:\app\519\pico\pico-sdk> git submodule update --init
PS D:\app\519\pico\pico-sdk> cd ..
PS D:\app\519\pico> git clone -b master https://github.com/raspberrypi/pico-examples.git
```

# Building "Hello World" from Visual Studio Code
Firstly, open the Developer Command Prompt for VS 2022 and type,

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/hw%201.PNG" width="500px">

From this way, Visual Studio will be open with all correct environment.

Then, this is a setting part. 
Choose Setting

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/hw%202.PNG" width="500px">
