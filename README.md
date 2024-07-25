# nRF DTM

<img src="https://github.com/olleheugene/nRF-DTM/blob/master/pics/DTM_USAGE.gif">

The nRF DTM is a UI-based standalone RF test tool designed for ease of controlling RF Test features of the nRF5 series of Nordic semiconductor.

Supporting features are 
- UI based RF test tool
- Bluetooth 5 features (2Mbps/Coded S8/Coded S2/1Mbps)
- Bluetooth 5.1 DF features (AoA/AoD)
  - The nRF DTM tool supports both AoA/AoD but the DTM Firmware  in nRF5 SDK only supports AoA Tx
  - refer to the [AoA TX test result](https://github.com/olleheugene/nRF-DTM/wiki/AoA-test-result)
- Bluetooth 5.2's Tx power control feature
- Listing the supported features
- Selectable UART Baudrates
- 3 sequential channels testing   (High/Mid/Low)
- Nordic Vendor-specific commands (Tx Power / Constant Carrier )
- PER measurement
- Listing DTM available serial port(s)
- Average RSSI measurement (Firmware modification required)
- Configurable log level to check the test sequence and details
- [configurable settings with .ini](Release/Windows/nrfdtm_config.ini)
- Integrated test guide
- Selectable physical and link-layer channel map
  - The Bluetooth's [Link layer channel list](https://github.com/olleheugene/nRF-DTM/raw/master/pics/link_channels_org.png)
  - The Bluetooth's [Physical layer channel list](https://github.com/olleheugene/nRF-DTM/raw/master/pics/physical_channels_org.png)
- Support multiple OS (macOS/Windows/Ubuntu)

# Getting Started
To learn more about nRF DTM, please visit [wiki](https://github.com/olleheugene/nRF-DTM/wiki) page

# How to modify the firmware source code to support the average RSSI measurement
- [Code Changes](https://github.com/olleheugene/nRF-DTM/wiki/Code-Changes)

# Download the latest version
- [For Windows 32bit](https://github.com/olleheugene/nRF-DTM/raw/v2.6.1/Release/Windows_x86/nRF_DTM_x86.exe)  (available in 2.x.x versions only)
- [For Windows 64bit](https://github.com/olleheugene/nRF-DTM/raw/master/Release/Windows/nRF_DTM.exe)  
- [For Ubuntu](https://github.com/olleheugene/nRF-DTM/raw/master/Release/Ubuntu/nRF_DTM)  
- [For macOS](https://github.com/olleheugene/nRF-DTM/raw/master/Release/macOS/nRF_DTM)

# Attention 
This tool is not an official Nordic tool that planned, developed, and production level verification by the Nordic semiconductor.
Personal project for providing better usage.


All bug reports, feedbacks are welcome.
