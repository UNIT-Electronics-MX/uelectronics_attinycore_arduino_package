# uElectronics ATTinyCore Package - DevLab Edition

Arduino Package for ATtiny MCUs - Optimized for DevLab Development Boards

This is a custom Arduino package based on [ATTinyCore](https://github.com/SpenceKonde/ATTinyCore) by Spence Konde, specifically optimized for UNIT Electronics DevLab development boards.

---

## Installation

### Method 1: Arduino IDE (Recommended)

1. Open Arduino IDE
2. Go to **File → Preferences**
3. In "Additional Boards Manager URLs" add:

```
https://raw.githubusercontent.com/UNIT-Electronics-MX/uelectronics_attinycore_arduino_package/refs/heads/v2.0.0-devThis-is-the-head-submit-PRs-against-this/package_uelectronics_attiny_custom.json
```

4. Go to **Tools → Board → Boards Manager**
5. Search for "uElectronics ATTiny Core"
6. Click "Install"

### Method 2: Manual Installation

Download the package from [Releases](https://github.com/UNIT-Electronics-MX/uelectronics_attinycore_arduino_package/releases) and extract it to your Arduino hardware folder.

---

## DevLab Special Features

### ATtiny88/48 DevLab Board

This version includes optimized support for the **ATtiny88/48 DevLab** board with the following features:

- USBasp programmer configured by default
- LED_BUILTIN assigned to PD0 (optimized for DevLab hardware)
- All standard clock and configuration options
- Compatible with DevLab shields and modules

### Board Configuration

```
Tools → Board → uElectronics ATTiny Core → ATtiny88/48 DevLab (USBasp)
```

**Recommended settings:**
- **Chip**: ATtiny88
- **Clock**: 8 MHz (internal) or according to your hardware
- **Programmer**: USBasp (already configured by default)
- **BOD**: 2.7V (recommended for stability)

---

## Supported Microcontrollers

This package maintains full compatibility with the original ATTinyCore chips:

- ATtiny25/45/85
- ATtiny24/44/84
- ATtiny441/841
- ATtiny261/461/861
- ATtiny87/167
- ATtiny48/88 (with DevLab variant)
- ATtiny2313/4313
- ATtiny1634
- ATtiny828
- ATtiny43
- ATtiny26

---

## Differences from Original ATTinyCore

### DevLab Optimizations:
1. **More compact package** - Reorganized files for faster installation
2. **USBasp default configuration** for DevLab boards
3. **LED_BUILTIN remapped** for DevLab hardware (PD0 instead of PB5)
4. **Bilingual documentation** (Spanish/English)
5. **Download URLs from UNIT Electronics GitHub Releases**

### Compatibility Maintenance:
- Full original ATTinyCore functionality
- Same bootloader options (Optiboot, Micronucleus)
- Same clock and fuse options
- Compatible with existing sketches

---

## Using with USBasp Programmer

DevLab boards are designed to work with USBasp programmers. Configuration is already included:

1. Connect your USBasp programmer to the DevLab board
2. Select the board: **ATtiny88/48 DevLab (USBasp)**
3. Use **Sketch → Upload Using Programmer**

Or simply press **Ctrl+Shift+U**

---

## Additional Resources

- [UNIT Electronics Website](https://uelectronics.com)
- [Original ATTinyCore Documentation](https://github.com/SpenceKonde/ATTinyCore)
- [DevLab Hardware Repository](https://github.com/UNIT-Electronics-MX)
- [Support and Discussions](https://github.com/UNIT-Electronics-MX/uelectronics_attinycore_arduino_package/discussions)

---

## License

This project inherits the license from the original [ATTinyCore](https://github.com/SpenceKonde/ATTinyCore) project:

- **Core files**: LGPL 2.1
- **Examples and documentation**: Creative Commons Attribution-ShareAlike 3.0

DevLab-specific modifications maintain the same license.

### Acknowledgments

This package is based on the excellent work of **Spence Konde** ([ATTinyCore](https://github.com/SpenceKonde/ATTinyCore)). 

We greatly appreciate his contribution to the Arduino and AVR community.

---

## Bug Reports

For DevLab-specific modification issues:
- [Issues in this repository](https://github.com/UNIT-Electronics-MX/uelectronics_attinycore_arduino_package/issues)

For original ATTinyCore functionality problems:
- [Issues in original ATTinyCore](https://github.com/SpenceKonde/ATTinyCore/issues)

---

## Updates

**Current version:** 3.0.0 (2026-01-09)

### Latest changes:
- Support for ATtiny88/48 DevLab board with USBasp
- LED_BUILTIN configured on PD0 for DevLab hardware
- Optimized and compressed package
- Distribution system via GitHub Releases

---

## Contributing

Contributions are welcome. Please:
1. Fork the repository
2. Create a branch for your feature
3. Submit a Pull Request

---

**Developed by [UNIT Electronics](https://uelectronics.com)**

**Based on ATTinyCore by Spence Konde**
