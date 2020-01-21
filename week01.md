# AY2020_ID2116 w01 micro:bit intro

# BBC micro:bit

https://microbit./

The **Micro Bit** (also referred to as **BBC Micro Bit**, stylized as **micro:bit**) is an [open source hardware](https://en.wikipedia.org/wiki/Open_source_hardware) [ARM](https://en.wikipedia.org/wiki/ARM_architecture)-based [embedded system](https://en.wikipedia.org/wiki/Embedded_system) designed by the [BBC](https://en.wikipedia.org/wiki/BBC) for use in computer education in the [UK](https://en.wikipedia.org/wiki/United_Kingdom).

https://www.youtube.com/watch?v=Wuza5WXiMkc&

----------
## micro:bit hardware architecture
![](https://microbit.org/images/microbit-hardware-access.jpg)

|                                                                                                         | **micro:bit**                                                                                                                               |
| ------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| **Processor**                                                                                           | nRF51822, 16 MHz 32bit-ARM Cortex microcontroller,                                                                                          |
| **Memory**                                                                                              | 256 KB Flash, 16 KB RAM                                                                                                                     |
| **Network**                                                                                             | **Bluetooth LE**, Nordic Radio, USB, Serial, SPI, I2C                                                                                       |
| **Sensor**                                                                                              | - Push Button x 2<br>- Digital Compass<br>- 3-axis Accelerometer<br>- Light Sensor<br>- Temperature Sensor                                  |
| **Display**                                                                                             | 5x5 LED light matrix                                                                                                                        |
| **Digital I/O Pins**<br><br>![](https://os.mbed.com/media/uploads/JonnyA/microbit_platform_image_2.png) | GPIO x 17<br><br>- 2/3 reconfigurable PWM outputs<br>- 5 x Banana/Croc-clip connectors<br>- Edge connector<br>- 6 x Analog In<br>- max 90mA |
| **Operating Voltage**                                                                                   | 1.8v ~ 3.3v (AAA battery x 2 )                                                                                                              |
| **Dimensions**                                                                                          | 5cm(w) 4cm(h)                                                                                                                               |
| **Weight**                                                                                              | 5g                                                                                                                                          |



## micro:bit Programming Languages
| **language**                | **online editor**                                                                                                             | **screenshot**                                                                                                                                                 |
| --------------------------- | ----------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **CodeBlocks / JavaScript** | https://makecode.microbit.org/#editor <br><br>- Reference<br>    - https://makecode.microbit.org/reference                    | ![](https://paper-attachments.dropbox.com/s_B95BABF9A570D80A8E913AFB210B9F88C60026D15B8090117F5DFFF2CA91F2E3_1579152664328_panel01.png)                        |
| **Python**                  | https://python.microbit.org/v/2.0<br><br>- Reference <br>    https://microbit-micropython.readthedocs.io/en/latest/index.html | ![](https://paper-attachments.dropbox.com/s_B95BABF9A570D80A8E913AFB210B9F88C60026D15B8090117F5DFFF2CA91F2E3_1579159463766_Screenshot+2020-01-16+15.23.24.png) |
| **C++**                     | https://os.mbed.com/platforms/Microbit/                                                                                       | ![Image result for mbed.com online compiler microbit](https://os.mbed.com/media/uploads/jplunkett/select-platform.png)                                         |

## CodeBlocks: Visual Programming 
![User-uploaded image: panel01.png](https://paper-attachments.dropbox.com/s_B95BABF9A570D80A8E913AFB210B9F88C60026D15B8090117F5DFFF2CA91F2E3_1579152664328_panel01.png)



## World of CodeBlocks
- **Arduino**: 
    - AutoDesk TinkerCad
     https://www.tinkercad.com/things/6zw6hKX60aq-super-krunk-sango/editel?tenant=circuits
- **Desktop, iOS App:** 
    - Scratch https://scratch.mit.edu/
- **Android App**: 
    - App Inventor https://appinventor.mit.edu/
- **Robot Programming:** 
    - DJI RoboMaster https://www.dji.com/sg/robomaster-s1


## Blocks
![](https://paper-attachments.dropbox.com/s_B95BABF9A570D80A8E913AFB210B9F88C60026D15B8090117F5DFFF2CA91F2E3_1579240264603_Input01.png)
![](https://paper-attachments.dropbox.com/s_B95BABF9A570D80A8E913AFB210B9F88C60026D15B8090117F5DFFF2CA91F2E3_1579240281611_Loops.png)

## [Hands-On 01] [Hello World](https://makecode.microbit.org/_AYEfFsh6oXDa)
1. Open Micro:Bit Editor and create a following code ( https://makecode.microbit.org/#editor)
| **CodeBlocks**<br>https://makecode.microbit.org/#editor                                                                                   | ![](https://paper-attachments.dropbox.com/s_B95BABF9A570D80A8E913AFB210B9F88C60026D15B8090117F5DFFF2CA91F2E3_1579162398992_file.png) |
| ----------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| **JavaScript**<br>https://makecode.microbit.org/#editor<br><br>![](https://www.dropbox.com/s/hbab2i7qex4qnfm/BlocktoJavaScript.png?raw=1) | ![](https://paper-attachments.dropbox.com/s_B95BABF9A570D80A8E913AFB210B9F88C60026D15B8090117F5DFFF2CA91F2E3_1579162777490_file.png) |
| **Python**<br>https://python.microbit.org/v/2.0                                                                                           | from microbit import *<br><br>while True:<br>    display.scroll('Hello, World!')<br>    display.show(Image.HEART)<br>    sleep(2000) |

## Uploading a program to a micro:bit

**01: The basic steps:**
https://makecode.microbit.org/device/usb
Download .hex program and upload to the device. (**SAFE, GOOD FOR PRODUCTION**).  

1. Connect your micro:bit to your computer with a USB cable.
2. Click **Download** to download the `.hex` file.
3. Move the `.hex` file from your computer onto the **MICROBIT** drive. The next section has instructions for the browser that you’re using.

**02: Pairing micro:bit to the editor** 
Upload the program directly to the device (**FASTER**). 

![1. Click Setting → Pair Device](https://paper-attachments.dropbox.com/s_B95BABF9A570D80A8E913AFB210B9F88C60026D15B8090117F5DFFF2CA91F2E3_1579229903293_pairdevice01.png)
![2. Click Pair device](https://paper-attachments.dropbox.com/s_B95BABF9A570D80A8E913AFB210B9F88C60026D15B8090117F5DFFF2CA91F2E3_1579229903308_pairdevice02.png)
![3. Select your micro:bit](https://paper-attachments.dropbox.com/s_B95BABF9A570D80A8E913AFB210B9F88C60026D15B8090117F5DFFF2CA91F2E3_1579229916546_pair03.png)

![4. Hit Donload button](https://paper-attachments.dropbox.com/s_B95BABF9A570D80A8E913AFB210B9F88C60026D15B8090117F5DFFF2CA91F2E3_1579230090793_download.png)



## [Hands-On 02] [H](https://makecode.microbit.org/_AYEfFsh6oXDa)eartBeat


![](https://paper-attachments.dropbox.com/s_B95BABF9A570D80A8E913AFB210B9F88C60026D15B8090117F5DFFF2CA91F2E3_1579152692518_Tutorial002.png)



## Loops
![](https://www.dropbox.com/s/86f4onord019mp7/Loops.png?raw=1)
![](https://paper-attachments.dropbox.com/s_E27A71D68A8DD03433A28687C5B4A68A9D179B868137B5C11A21CC29DD2B56DA_1548383700416_Arduino+Tutorial_Page_61.jpg)



## [Hands-On 03] [H](https://makecode.microbit.org/_AYEfFsh6oXDa)eart Beat with timed delay

By adding pause, you can delay the timing to move to the next block.
**Try: changing the number. e.g. 100 , 10000**

![](https://paper-attachments.dropbox.com/s_B95BABF9A570D80A8E913AFB210B9F88C60026D15B8090117F5DFFF2CA91F2E3_1579163313904_Tutorial003.png)

# Variables: 
![](https://www.dropbox.com/s/cbf84kx31iwrgxf/Variables.png?raw=1)
![](https://www.dropbox.com/s/bqgpyx0zm3vf45q/Variable.jpg?raw=1)



## [Hands-On 04] [H](https://makecode.microbit.org/_AYEfFsh6oXDa)eart Beat with Variables

By introducing a variable, you can change/reuse values in the code at once.
**Try: changing the delayTime, e.g 100, 10000**

![](https://paper-attachments.dropbox.com/s_B95BABF9A570D80A8E913AFB210B9F88C60026D15B8090117F5DFFF2CA91F2E3_1579163361091_Tutorial004.png)

## [Hands-On 05] Simple Counter


![](https://paper-attachments.dropbox.com/s_B95BABF9A570D80A8E913AFB210B9F88C60026D15B8090117F5DFFF2CA91F2E3_1579163382665_Tutorial005.png)


Try **: Modify the code to count down when button A is pressed**

# Conditionals:  IF-Else Statement
![](https://paper-attachments.dropbox.com/s_E27A71D68A8DD03433A28687C5B4A68A9D179B868137B5C11A21CC29DD2B56DA_1548389193510_IF_microbit.png)
![](https://paper-attachments.dropbox.com/s_E27A71D68A8DD03433A28687C5B4A68A9D179B868137B5C11A21CC29DD2B56DA_1548389193502_IF_JavaScript.png)



## [Hands-On 06] Conditionals


![](https://paper-attachments.dropbox.com/s_E27A71D68A8DD03433A28687C5B4A68A9D179B868137B5C11A21CC29DD2B56DA_1548386804211_Ex01_FeelingNumerical.png)




# Sensors 


## [Hands-On 05] Temperature Sensor 
![](https://paper-attachments.dropbox.com/s_B95BABF9A570D80A8E913AFB210B9F88C60026D15B8090117F5DFFF2CA91F2E3_1579234299907_file.png)


**Try: Instead of displaying temperature value, use conditional(if-else) to show**
        **if  temperature >= 30, display “Hot!”**  
        **if  temperature < 0, display “Cold!”** 
        **else temperature: display temperature** 




