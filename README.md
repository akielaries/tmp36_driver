# TMP36 Driver
This repo contains a generic TMP36 driver but also an application for using the TMP36 sensor as
an onboard sensor on the BeagleBone Black. The BeagleBone Black's AM335x ARMv7 processor does not contain 
an onboard temperature sensor other than the silicon bandgap temperature sensor used in testing/QA but
NOT accessible to users in any way. 

This project does 2 things:

1. Implements a driver for the TMP36 sensor
2. Implements a temperature sensor driver in place of `/sys/class/hwmon` or `/sys/class/thermal` on
devices lacking such functionality
