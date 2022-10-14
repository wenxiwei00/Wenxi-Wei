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
* PuTTY

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

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/4.1.PNG" width="500px">

# Git
Download from https://git-scm.com/download/win.

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/5.1.PNG" width="500px">

# Getting the SDK and examples
Open **Visual Studio Code >> Terminal >> New Terminal**.
Initial the address
```
PS D:\app\519\pico\pico-examples> cd "D:\app\519\pico"
```
<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/6.1.PNG" width="500px">

Then, clone SDK and example from github
```
PS D:\app\519\pico> git clone -b master https://github.com/raspberrypi/pico-sdk.git  
PS D:\app\519\pico> cd pico-sdk
PS D:\app\519\pico\pico-sdk> git submodule update --init
PS D:\app\519\pico\pico-sdk> cd ..
PS D:\app\519\pico> git clone -b master https://github.com/raspberrypi/pico-examples.git
```

# Building "Hello World" from Visual Studio Code
Firstly, open the **Developer Command Prompt for VS 2022** and type,

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/hw%201.PNG" width="500px">

From this way, Visual Studio Code will be open with all correct environment.

Then, install the **CMake Tools** extension. Click on **Extension in the left-hand toolbar >> search **CMake Tools >> click on entry in the list >> click on the install button**

Next, click on the Cog Wheel at the bottom of the navigation bar on the left-hand side of the interface and select **setting**.

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/hw%202.PNG" width="500px">

In the setting pane, **click Extensions >> CMake Tools >> CMake: Configure Environment >> Add Item >> set the PICO_SDK_PATH to be ..\..\pico-sdk**.

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/hw%203.PNG" width="500px">

Scroll down to **Cmake: Generator** and enter **NMake Makefiles**

Next, go to the file menu. **Open File >> choose pico-example >> Select Folder**. When you are prompted to configure the project which will show on right bottom, select **GCC for arm-none-eabi** for your compiler.

Go ahead and click on the **Build button** (with a cog wheel) in the blue bottom bar of the window. This will create the build directory and run CMake and build the examples project, including "Hello World".

Then, your computer will exist a file called **hello_usb.uf2** inside the build folder.

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/hw%204.PNG" width="500px">

The next step is connecting Adafruit QT Py RP2040 to computer and drag **hello_usb.uf2** into Adafruit QT Py RP2040. After inserting QT Py RP2040, hold down the **BOOT/BOOTSEL button** (highlighted in red), and while continuing to hold it (don't let go!), press and release the **reset button** (highlighted in blue). Continue to hold the BOOT/BOOTSEL button until the RPI-RP2 drive appears.

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/hw%205.PNG" width="500px">

Then drag the **hello_usb.uf2** into Adafruit QT Py RP2040 drive.

# PuTTY
Download **PuTTY** from https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/putty%202.PNG" width="500px">

Open **device manager** in your computer to make sure what port QT Py RP2040 is connected to.

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/putty%201.PNG" width="500px">

Open **PuTTY** and set the following parts (highlighted in yellow).

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/putty%203.PNG" width="500px">

Then, the "Hello World" shows on PuTTY.

<img src="https://github.com/wenxiwei00/Wenxi-Wei/blob/main/putty%204.PNG" width="500px">






