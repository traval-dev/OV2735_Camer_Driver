# OV2735_Camera_Driver

Linux kernel driver for the OmniVision OV2735 camera sensor.

## Overview

This repository provides the V4L2 subdevice driver for the OV2735 image sensor, intended for use with platforms supporting MIPI CSI-2 input, such as the NXP i.MX8M Plus-based **Debix Model A**.

## Tested Environment

- **Platform**: Debix Model A  
- **Kernel Version**: 6.14-rc6  
- **Interface**: MIPI CSI-2  
- **Bus**: I2C  
- **Driver Type**: V4L2 sensor subdevice  
- **Format**: RAW Bayer (example: RAW10)

## Features

- Supports power-up/down sequences
- Supports V4L2 control framework (exposure, gain, etc.)
- Implements async device binding
- Compliant with Linux kernel driver model
- Proper error handling with `cci_write()`/`cci_read()`
