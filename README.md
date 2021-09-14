# nRF DTM

<img src="https://github.com/olleheugene/nRF-DTM/blob/master/pics/DTM_USAGE.gif">

nRF DTM is UI based Standalone RF test tool for the Nordic nRF5 series.
It provides ease of control for configuring RF setting as channels, Tx power, etc.

Supporting features are 
- UI based RF test tool
- Bluetooth 5 features (2Mbps/Coded S8/Coded S2/1Mbps)
- Bluetooth 5.1 DF features (AoA/AoD)
  - Supports both AoA/AoD but DTM Firmware (nRF5 SDK v17.0.1/NCS v1.6) only supports AoA Tx
  - refer to the AoA TX test result
- Bluetooth 5.2 Tx power control feature
- Listing the supported features
- Sequential 3 channels testing   (High/Mid/Low)
- Nordic Vendor specific commands (Tx Power / Constant Carrier )
- PER measurement
- Average RSSI measurement (Firmware modification required)
- Configurable log level to check the test sequence and details
- Selectable physical and link layer channel map
  - The Bluetooth's [Link layer channel list](https://github.com/olleheugene/nRF-DTM/blob/master/pics/link_channels_org.png)
  - The Bluetooth's [Physical layer channel list](https://github.com/olleheugene/nRF-DTM/blob/master/pics/physical_channels_org.png)
- Supports Windows /Ubuntu 20.04 / macOS

# Getting Started
To learn more about nRF DTM, please visit [wiki](https://github.com/olleheugene/nRF-DTM/wiki) page

# How to modify the firmware source code to support the average RSSI measurement
- [Code Changes](https://github.com/olleheugene/nRF-DTM/wiki/Code-Changes)

# Download the latest version
- [For Windows 32bit](https://github.com/olleheugene/nRF-DTM/raw/master/Release/Windows_x86/nRF_DTM_x86.exe)  
- [For Windows 64bit](https://github.com/olleheugene/nRF-DTM/raw/master/Release/Windows_x64/nRF_DTM_x64.exe)  
- [For Ubuntu 20.04](https://github.com/olleheugene/nRF-DTM/raw/master/Release/Ubuntu/nRF_DTM_x64_ubuntu)  
- [For macOS](https://github.com/olleheugene/nRF-DTM/blob/master/Release/macOS/nRF_DTM_x64_macOS)

# Attention 
This tool is not an official Nordic tool that planned, developed, and production level verification by the Nordic semiconductor.
Personal project for providing better usage.


All bug reports, feedbacks are welcome.
