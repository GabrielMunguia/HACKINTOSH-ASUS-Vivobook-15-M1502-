# ASUS Vivobook 15 (M1502) Hackintosh EFI

This project contains the EFI configuration for running macOS on an ASUS Vivobook 15 (M1502) laptop. The configuration has been tested and confirmed to work on macOS Sonoma and macOS Ventura.

## Laptop Specifications

- **Processor**: AMD Ryzen 5 4600H
- **Graphics**: AMD Vega 6
- **RAM**: 16GB
- **Storage**: 256GB M.2 SSD

## Features

### Working Components

- **Graphics Acceleration**: Fully functional graphics acceleration, providing smooth system performance.
- **Sound**: Sound works correctly, with support for internal speakers and headphones.
- **Bluetooth**: Bluetooth is operational, allowing connections to external devices such as keyboards, mice, and headphones.

### Known Issues

- **Wi-Fi**: Wi-Fi is currently not working. We are working on a solution to enable it in future updates.

## Compatibility

- **macOS Sonoma**
- **macOS Ventura**

## Installation

1. Download this repository.
2. Copy the `EFI` folder to the root directory of your macOS installation USB.
3. Ensure you configure your BIOS settings according to standard Hackintosh recommendations.
4. **Important:** You must generate a custom SMBIOS using `GenSMBIOS` with the `MacBookPro16,3` model. Using the default or an incorrect SMBIOS will cause issues during installation or with system stability.
   - Run `GenSMBIOS` and select the `MacBookPro16,3` option to generate a new SMBIOS.
   - Replace the existing SMBIOS information in the `config.plist` file with the newly generated values.
5. Install macOS on your ASUS Vivobook 15 (M1502) using the prepared USB.

## Notes

- Please back up your system before making any modifications.
- This project is in development, and some features may not be fully implemented or may be unstable.

## Contributions

If you have found a solution for any of the mentioned issues or want to contribute in any other way, feel free to submit a pull request!

## License

This project is distributed under the MIT License. You are free to use and modify it, but no warranty is provided for its functionality across all systems.
