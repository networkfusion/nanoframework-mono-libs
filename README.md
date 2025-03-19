# Mono repo for .Net nanoFramework managed libraries.
All libraries are added as submodules for independent (stamped) updates.
The CoreLibrary and all its depend libraries are contained in the `lib` directory.


## lib
This directory contains all managed (csharp) core libraries for .NET nanoFramework.

### It does not contain the following project repos:

#### SDK/Firmware related:
* ChibiOS-Contrib
* mbedtls
* nf-Community-Targets
* nf-interpreter
* SimpleLink_CC13xx_26xx_SDK
* SimpleLink_CC32xx_SDK
* STM32CubeF0
* STM32CubeF4
* STM32CubeF7
* STM32CubeH7
* STM32CubeL0
* STM32CubeL4
* TI_SysConfig
* TI_XDCTools

#### VS Extension / deployment related:
* hex2dfu
* metadata-processor
* nanoFirmwareFlasher
* nf-debugger
* nf-Visual-Studio-extension
* nf-VSCodeExtension

#### Test related:
* nanoFramework.Benchmark
* nanoFramework.IoT.TestStream
* nanoFramework.TestFramework

#### Github Actions:
* nanobuild (GitHub Action to install .NET nanoFramework build components.)
* nanodu (GitHub Action to update NuGet references of .NET nanoFramework projects.)

#### Project management:
* .github (This is the general template and configuration for the .NET nanoFramework GitHub organization.)
* Home (The landing page for .NET nanoFramework repositories.)
* nanoframework.github.io (repository for .NET nanoFramework documentation web site.)
* nFBot (Discord bot for .NET nanoFramework Discord server.)
* nf-tools (Various CI management tools.)

#### Not deemed necessary as part of a core update process:
* nanoFramework.MXCHIP (repo empty)
* nf-Community-Contributions
* Samples

#### Obsolete (deprecated / archived) repositories:
* esp32-firmware-flasher
* Json.NetMF
* nanoFramework.System.Runtime
* nanoFrameworkDeployer
* Windows.Devices.Adc
* Windows.Devices.Gpio
* Windows.Devices.I2c
* Windows.Devices.Pwm
* Windows.Devices.SerialCommunication
* Windows.Devices.Spi
* Windows.Storage
* Windows.Storage.Streams


## Update submodules
To update ALL submodules to the latest versions, use `git submodule update --remote` from the terminal.  
To update individual submodules, change to its respective directory and perform a `git pull`.

Changes for each submodule can be adjusted or reverted before they are commited.
