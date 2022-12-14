# rtl8703bs_rtl8723cs_driver_solo
Linux driver for rtl870bs/rtl8723cs Realtek wifi chips. 
extracted from https://github.com/megous/linux/tree/wifi-6.1 and modified in order to be built for mainline (6.1) linux kernel

rtl8703bs and rtl8723cs are pin to pin compatible chips (from what I've found on the Internet), hence this driver can be build and used in both cases.


In order to build the driver, run the following command from within rtl8723cs directory:
`make -j4 ARCH=arm CROSS_COMPILE=arm-linux-gnueabihf- KSRC=<PATH_TO_LINUX_DIR> M=$PWD`