# Hardware
This repository is intended for hardware design for the CR-6 SE 3D-printer.

## Current hardware projects:

### CR-6 SE Hot end circuit board community edition V0.1 - Stock Creality CR6

The CR-6 SE hot end circuit board community edition is a reverse engineered circuit board based on the Creality board. The intention behind it's release is to make the design opensource and encourage further development of the strain gauge bed levelling system and to allow alternate circuit boards for custom hot ends. This sub repository contains the following files:
* Circuit board schematics
* Circuit board layouts
* Datasheets of used components
* Production files for circuit board manufacturing
* Manual containing:
   * How to order the circuit board;
   * How to flash firmware on the circuit board;
   * How to install the circuit board;
   * How to test and calibrate the circuit board.
 
 Make sure to read the manual first.

### CR-6 SE Hot end circuit board community edition V0.21 - 12V/BLTOUCH edition

This design removes the strain gauge levelling method and implements the 3-pin and 2-pin connectors to connect a BLTOUCH probe. It also has an optional 12VDC/1A buck converter in case 12VDC fans are used. The Fan Voltage (V_FAN) can be selecting by placing a jumper on the V_FAN selection header connecting either 24VDC and V_FAN or 12VDC and V_FAN.

Please note that a changed Marlin version needs to be flashed on the motherboard where the functions of the PROBE_TARE_PIN should change to a PWM output for the BLTOUCH servo and the Z_STOP_PIN pin should be customized for BLTOUCH ZMIN.
