# BluetoothDeviceDiscovery
 A repository for the Lab 2.4.7 project on discovering Bluetooth devices for the TestOut CyberDefense Pro CompTia course.
# Bluetooth Device Discovery Lab

## Overview
This project documents the steps and procedures for discovering Bluetooth devices within a corporate network and gathering information about them. As a security analyst, the goal is to protect Bluetooth devices from potential attacks and understand the devices running in the company network.

## Lab Scenario
In this lab, we performed the following tasks using terminal commands:

1. Use `hciconfig` to discover and enable the onboard Bluetooth adapter.
2. Use `hcitool` to find all Bluetooth devices.
3. Answer Question 1: As a result of the scan, how many devices were found? (Your answer: 6)
4. Use `l2ping` to determine if Bluetooth devices are up and in range.
5. Answer Question 2: How many of the devices scanned were alive and in range? (Your answer: 6)
6. Use `sdptool` to query a specific laptop to determine available Bluetooth services.
7. Answer Question 3: Which service searches were successful on Francisco's Precision Laptop? (Your answer: Ad Hoc User Service, Device ID Service Record)
8. Use `hcitool` to determine the clock offset and class for a specific Bluetooth speaker device.
9. Answer Question 4: Using the MAC address, what is the class ID number for Brian's Braven speaker? (Your answer: 0x248080)

## Additional Helpful Commands
Here are some additional helpful commands used during the lab:

- `hciconfig --help`: Get help and information about `hciconfig` command.
- `hciconfig hci0 up`: Start the Bluetooth device.
- `hcitool scan`: Scan for Bluetooth devices.
- `hci inq`: Inquire for Bluetooth devices.

## Requirements
- Linux environment (this lab assumes Linux-based commands).
- Administrative privileges may be required for certain commands.

## Usage
Follow the steps below to perform the lab tasks:

### Step 1: Discover and Enable Bluetooth Adapter
Use the following commands to enable the Bluetooth adapter:
```shell
hciconfig
hciconfig hci0 up
hciconfig
