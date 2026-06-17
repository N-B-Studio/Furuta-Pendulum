# Furuta Pendulum (STM32H753ZI)

Short demo project for the Furuta (rotary inverted) pendulum running on an STM32H753ZI board.

![Furuta Pendulum 3D model](3D%20file/image.jpg)

**Overview:**
- This repository contains firmware, board support and project files for the Furuta Pendulum built with STM32CubeIDE targeting the STM32H753ZITx MCU.
- The project includes HAL drivers, startup code and a sample `main` application under `Core/`.

**Quick start**
1. Install STM32CubeIDE and the STM32H7 HAL package.
2. Open the project file `H753ZI-Furuta-Pendulum.ioc` in STM32CubeIDE (top-level folder).
3. Build the project using the IDE build button or via the provided makefile in `Debug/`.
4. Connect a compatible ST-Link and flash the generated `.elf`/`.bin` from the Debug output.

**Useful files**
- Project configuration: H753ZI-Furuta-Pendulum.ioc
- Linker scripts: STM32H753ZITX_FLASH.ld, STM32H753ZITX_RAM.ld
- Sources: [Core/](Core/)
- Image used in this README: [3D file/image.jpg](3D%20file/image.jpg)

**Build from command line (example)**
```powershell
cd "d:\z-code\STM32CubeIDE\Furuta-Pendulum\Debug"
make all
```

**Flash with STM32CubeProgrammer**
1. Build the project in STM32CubeIDE (or using `make`).
2. Open STM32CubeProgrammer, connect to the target and program the `*.bin` or `*.elf` file from the Debug output folder.

**License**
See the repository `LICENSE` file for licensing details.

If you want, I can also add a brief hardware BOM, wiring diagram, or build badges. Tell me which you'd like next.
