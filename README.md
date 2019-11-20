## Introduction

---

<p><img src=".\Resource_DTM_Guide\clip_image002.jpg"></p>  
The nRF_DTM is UI based test tool that helping to RF test by easy control

- UI based RF test tool
- Support Bluetooth 5 features (2Mbps/Coded S8/Coded S2/1Mbps)
- Support 3 Different channels testing (High/Mid/Low)
- Configurable Tx Power
- Support PER measurement
- Support configurable log level in order to check test sequence and detiails
- Support direct command on terminal and command line interface on shell









## How to use UI based NRF DTM

---

#### Basic environment

![1552528713853](.\Resource_DTM\1552528713853.png)

- Connect PC and Target board through USB to UART converter
- Nomally 4 lines needed for UART
  - UART Tx / Rx
  - VCC
  - GND
- <font color=red>Recommend connects USB-to-UART after connected VCC on target board </font>

#### Transmitter Test

1. Select connected COM port 

2. Configure Channel, Tx power, PHY, Payload Model

   If you want  non-modulation testing, select 
   "Payload Model" to "Constant Carrier"

4. Set the "Run Time" for how long time you want to send packets

   <Font color=Blue>For infinite transmit test, set the "Run Time" to 0(Zero) </font>

5. Start Tx test with clicking "Start Button"

#### Receiver Test

1. Select connected COM port  

2. Configure Channel, PHY, Payload Model 

   If you want  non-modulation testing, select 
   "Payload Model" to "Constant Carrier"

4. Set the "Run Time" for how long time you want to receive packets

   <Font color=Blue>You can't set the "Run Time" to 0(Zero) due to PER calculation</font>

5. Start transmitting packets from peer device

6. Start Rx test with clicking "Start Button"

#### Feature Control

###### Log enable 

Menu > View > Select "Log window"

## Command Line based nRF DTM 

---

![1552546940038](.\Resource_DTM\1552546940038.png)

#### Direct Terminal command

For direct command execution on windows terminal

1. Start Window Terminal 

2. Type `nRF_DTM start` on prompt. 

   If you don't use anyother configuration, It will start Tx testing with default values.

   You can read the details of command by `nRF_DTM --help` or `nRF_DTM -h`

3. For infinite Transmit testing, you should stop the testing by typing  `nRF_DTM stop` command

   If you don't this, you can't do other testing

#### CLI shell

For command execution on shell based command line interface

1. Start Window Terminal 

2. Type `nRF_DTM cli` on prompt

3. You can run the commands set  when the prompt shown as below.

   Currently available commands are  "start/stop/showcfg"

   You can easily check the available commands by pressing tab key or typing "help"

   ![1552547619291](.\Resource_DTM\1552547619291.png)

4. You can check the detail of options by adding `--help` that whatever you want 

   ![1552548042311](.\Resource_DTM\1552548042311.png)

5. For example, 

   You can do trasmitter test as below command 

   (if the configuration is same as default you can omit that items)

   `DTM> start --port=COM5 --mode=0 --channel=19 --power=0 --model=3 --length=1 --phy=1 --time=1000 --level=0 --repeat=1` 

   or

   `DTM> start --port=COM5`

   



































## Simple test with development kit (Case 1)

---

#### Prerequisite 

![1552545829421](.\Resource_DTM\1552545829421.png)

- DK x 2EA 

- PC x 1EA or 2EA 

- nRF_DTM x 2EA

  

#### Test procedure

1. Start two "nRF DTM" that one for Transmitter(A) and the other one for  Receiver(B)

2. Set the A's nRF DTM as Transmitter and congifures Channel/Tx Power/Payload Model/PHY/Run Time

   ("Run time" item sets to "0" for infinite testing)

3. Set the B's nRF DTM as Receiver and congifures Channel/PHY/Run Time

   ("Run time" item sets to whatever you want)

4. Check the PER on B's nRF DTM after timer expired 























## Simple test with development kit (Case 2)

---

#### Preparation

- 2 x Development Kit (nRF52-DK, nRF51-DK, nRF52840-DK, nRF52840-Dongle )
- nRF Connect for Desktop
- nRF DTM

#### Recommend environment

- Windows 7 ~

- nRF52840 for Full Radio Test (2Mbps/Coded PHY/8dBm)

- The RSSI Viewer supports nRF52-DK,nRF52840-DK,nRF52840-Dongle only

  Test Environment

![1543299852168](C:/Users/Eugene/Google%20Drive/1.Nordic%20Semiconductor%20Korea/Common/02.NORDIC_KOREA_GuideDocument/Resource_DTM_Guide/1543299852168.png)

#### Test Procedure

1. Flash the DTM firmware to one(A) development Kit

2. Flash the RSSI Viewer to the other one(B) through nRF Connect for Desktop's RSSI Viewer

3. Start RSSI viewer

4. Connect A Devkti to nRF DTM

   - Set the nRF DTM as Transmitter and configures Channel, Payload Model, PHY etc....
   - Recommend that Payload is Constant carrier and Run time is 0

5. Start nRF DTM

6. If you start nRF DTM successfully the RSSI viewer will show as below picture.

   It can be used simple measurement of Tx power level or frequency shift(if it has big gap)

<p><img src="./Resource_DTM_Guide/1543300108933.png" width="50%" align="center"></p>
