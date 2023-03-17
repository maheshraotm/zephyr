.. _sip_svc_sample:

SiP SVC sample
##############

Overview
********

This sample demonstrates the usage of SiP SVC subsystem.This sample
performs a voltage value query from Secure Device Manager in Intel Agilex
SoC FPGA.

Caveats
*******

* SiP SVC subsystem relies on the firmware running in EL3 layer to be in compatible
  with protocol defined inside the SiP SVC subsystem used by the project.
* The sample application relies on the Trusted Firmware ARM firmware in
  intel Agilex SoC FPGA query the voltage levels in Secure Device Manager.

Building and Running
********************
For building the application:

.. zephyr-app-commands::
   :zephyr-app: samples/subsys/sip_svc
   :board: intel_socfpga_agilex_socdk
   :goals: build

For running the application the Zephyr image can be loaded in DDR memory
at address 0x00100000 and ATF BL31 at 0x00001000 from SD Card or QSPI Flash
in ATF BL2.

Sample Output
*************
.. code-block:: console

   *** Booting Zephyr OS build zephyr-v3.3.0-1058-g640e79f7cde8 ***
   Voltage is 0.853363v
   Voltage is 0.870819v
   Voltage is 0.861069v
   Voltage is 0.856918v
   Voltage is 0.845383v
   Voltage is 0.845871v
   Voltage is 0.858459v
