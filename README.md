# SJSU Badge Programs

## Getting started

clone the repository and initialize the submodules:

```bash
git clone https://github.com/acarrou/sjsu-badge-programs.git
```

## Installing the Pico SDK
The Pico SDK is a submodule of this repository, to initialize it run:

```bash
git clone -b master https://github.com/raspberrypi/pico-sdk.git
cd pico-sdk
git submodule update --init
cd ..
```

## Building the examples
create a build directory and run cmake:

```bash
mkdir build
cd build
export PICO_SDK_PATH=../pico-sdk
cmake ..
make
```

## Flashing the examples
Connect your Pico while holding the BOOTSEL button, it will appear as a mass storage device. Copy the uf2 file to the device and it will flash the Pico.