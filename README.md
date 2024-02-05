# Raspberry Pi Pico SDK Examples

## Getting started

clone the repository and initialize the submodules:

```bash
git clone 
```

## Building the examples
create a build directory and run cmake:

```bash
mkdir build
cd build
cmake ..
make
```

## Flashing the examples
Connect your Pico while holding the BOOTSEL button, it will appear as a mass storage device. Copy the uf2 file to the device and it will flash the Pico.