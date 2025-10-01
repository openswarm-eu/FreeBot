# FreeBot
Contains FreeBot files and source code.
The Hardware folder contains schematics for the various versions of the FreeBot board and associated evaluation boards.
The software folder contains the FreeBot subfolder, which contains the core functionality of FreeBot and reference implementation of the library for BLE control. 
The repository will keep being updated with designs for both hardware and software.


# Hardware revisions

| Version        | SoC      | Feather-header | Picture                                       |
|:--------------:|:--------:|:--------------:|:---------------------------------------------:|
| [v1.0a](#v10a) | nrf52840 | &cross;        |![Picture of CapBot v1.0a](images/cb_v1.0a.jpg)|
| [v1.1a](#v11a) | nrf52840 | &cross;        |![Picture of CapBot v1.1a](images/cb_v1.1a.jpg)|
| [v1.1b](#v11b) | nrf52840 | &check;        |![Picture of CapBot v1.1b](images/cb_v1.1b.jpg)|

## v1.0a

CapBot v1.0 has a physical switch (`SW4`) to cut the UART lines from the DAP-link on-board debugger.
This switch should be enabled when printing to a serial terminal over USB.

Furthermore, another physical switch (`SW3`) cuts the SWD lines used for programming the &micro;Processor.
This switch should be enabled in order to flash.

## v1.1a

Nothing special (yet).

## v1.1b

> [!WARNING]
> The pins `IO1`, `IO2` and `IO3` on the feather-header correspond with `D15`, `D16` and `SW2` respectively.
> Make sure that these are not shorted accidentally because of this.
> ![Schematic view](../img/cb-v1.1b-io-collision.png)


# Acknowledgement

Part of the source code in this repository is developed within the frame and for the purpose of the OpenSwarm project. This project has received funding from the European Unioan's Horizon Europe Framework Programme under Grant Agreement No. 101093046.

![OpenSwarm - Funded by the European Union](logos/ack.png)
