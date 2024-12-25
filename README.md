# nRF DTM (nRF DTM CLI)

The nRF DTM is a [UI-based](https://github.com/olleheugene/nRF-DTM/wiki/UI-based-test) or [Command line based](https://github.com/olleheugene/nRF-DTM/wiki/Direct-Terminal-Command) standalone RF test tool designed for ease of controlling RF Test features of the nRF5 series of Nordic Semiconductor.

### Features 

- UI based, and separate Command line based tool for Bluetooth RF test 

- Supports most of Bluetooth DTM RF test features (2Mbps/Coded S8/Coded S2/1Mbps/[AoA](https://github.com/olleheugene/nRF-DTM/wiki/AoA-test-result)/AoD/Tx power control)
- Supports listing supported DTM features of the device
- Supports high, middle, and low 3 different channel sequential test
- Supports Nordic vendor-specific commands (Tx Power / Constant Carrier )
- Supports PER measurement with configurable level to verdict pass/fail
- Listing DTM available serial port(s) and automatic selection for DTM device
- Average RSSI measurement (Firmware modification required)
- Configurable log level to check the test sequence and details
- Supports predefined configurations [configurable settings with .ini](Release/Windows/nrfdtm_config.ini)
- Integrated test guide
- Supports selectable channel map in [physical-layer](https://github.com/olleheugene/nRF-DTM/raw/master/pics/physical_channels_org.png) and [link-layer](https://github.com/olleheugene/nRF-DTM/raw/master/pics/link_channels_org.png) channels
- Support multiple OS (macOS/Windows/Ubuntu)



# UI-based nRF-DTM

<img src="https://github.com/olleheugene/nRF-DTM/blob/master/pics/DTM_USAGE.gif" width=80%>

https://github.com/olleheugene/nRF-DTM/wiki/UI-based-test



# Command line-based nRF-DTM
<img src="https://github.com/olleheugene/nRF-DTM/blob/master/pics/cli.gif" width=80%>
https://github.com/olleheugene/nRF-DTM/wiki/Direct-Terminal-Command



# Guide to modify firmware for RSSI measurement

- [Code Changes](https://github.com/olleheugene/nRF-DTM/wiki/Code-Changes)



# Download the latest version

### nRF-DTM

- [Windows 32bit](https://github.com/olleheugene/nRF-DTM/raw/v2.6.1/Release/Windows_x86/nRF_DTM_x86.exe)  (available in 2.x.x versions only)
- [Windows 64bit](https://github.com/olleheugene/nRF-DTM/raw/master/Release/Windows/nRF_DTM.exe)  / [ini file (default configuration file)](https://github.com/olleheugene/nRF-DTM/blob/master/Release/Windows/nrfdtm_config.ini)
- [Ubuntu](https://github.com/olleheugene/nRF-DTM/raw/master/Release/Ubuntu/nRF_DTM)  / [ini file (default configuration file)](https://github.com/olleheugene/nRF-DTM/blob/master/Release/Ubuntu/nrfdtm_config.ini)
- [macOS-Intel core](https://github.com/olleheugene/nRF-DTM/raw/master/Release/macOS/nRF_DTM)(tested w/ macOS 13 Ventura)  / [ini file (default configuration file)](https://github.com/olleheugene/nRF-DTM/blob/master/Release/macOS/nrfdtm_config.ini)

### nRF-DTM-CLI

- [Windows 64bit](https://github.com/olleheugene/nRF-DTM/blob/master/Release/Windows/nRF_DTM_CLI.exe)  / [ini file (default configuration file)](https://github.com/olleheugene/nRF-DTM/blob/master/Release/Windows/nrfdtm_config.ini)
- [Ubuntu](https://github.com/olleheugene/nRF-DTM/raw/master/Release/Ubuntu/nRF_DTM_CLI)  / [ini file (default configuration file)](https://github.com/olleheugene/nRF-DTM/blob/master/Release/Ubuntu/nrfdtm_config.ini)
- [macOS-Intel core](https://github.com/olleheugene/nRF-DTM/raw/master/Release/macOS/nRF_DTM_CLI)(tested w/ macOS 13 Ventura)  / [ini file (default configuration file)](https://github.com/olleheugene/nRF-DTM/blob/master/Release/macOS/nrfdtm_config.ini)

> To run the tool on macOS, hold down the "Control" key and click on the nRF_DTM.


# More details

To learn more about nRF DTM, please visit [wiki](https://github.com/olleheugene/nRF-DTM/wiki) page



# Attention 

This is a personal project for convenient use of DTM. 
Therefore, Nordic Semiconductor will not be provided with official support for this tool.


But all bug reports and feedback are welcome. :)
