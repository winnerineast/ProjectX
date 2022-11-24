# Device Simulator

## Features
* to simulate device/sensor to send message
* to support various protocol and default is MQTT

## Installation
Currently it's still under development and you have compile source code to use.

it can run with any OS (but don't try WSL2) with nodejs version 16.x only (higher version will has error:0308010C:digital envelope routines::unsupported).

```
# Clone
git clone the entire project

# Go to device simulator folder
cd ProjectX/device_simulator

# Install dependencies
yarn install

# Compiles for development trying
yarn run electron:serve

# build for production
yarn run electron:build
```
After the building is successful, the corresponding installation file for the successful building will appear in the dist_electron directory.

If you need to package it as an installation package for an independent operating system, please refer to the following commands to generate installation kit.
```
# Windows
yarn run electron:build-win
# Linux
yarn run electron:build-linux
#macOS
yarn run electron:build-mac
```