# Prebuilt Python Wheels for pylibpd

This repository provides prebuilt binary wheels for `pylibpd`, specifically tailored for modern Linux environments.

### Technical Specifications

* **Architecture**: x86_64
* **Platform**: Linux (Built on Arch Linux)
* **Build Tooling**: SWIG 4.x
* **Python Versions**:
* **3.13**: Built using a modernized SWIG interface utilizing the PEP 3118 Buffer Protocol (replaces deprecated legacy Buffer API).
* **3.12**: Standard build for stable environments.

### Build Configuration

These wheels are built as **Vanilla-only** versions of `libpd`. To ensure maximum compatibility and stability on rolling-release distributions, the "extra" externals (e.g., `fiddle~`, `sigmund~`) have been excluded from the binary to prevent linker errors and undefined symbol crashes.

### Installation

You can install the wheels directly via pip:

```bash
pip install pypdlib-0.14.0-cp313-cp313-linux_x86_64.whl

