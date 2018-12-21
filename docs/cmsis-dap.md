## CMSIS-DAP Tutorial



### Abstract



In this tutorial we  use CMSIS-DAP to program a MCB1700 board. We program a blinky example in Keil Uvision 5.



![](img/cmsis-dap/cmsisdap.png)





### Prerequisites



Make sure your CMSIS-DAP is running the correct [firmware](usbd_hid_dap.bin).



To install the firmware, first you have to trigger the bootloader by shorting the pads before powering up the board:



![](img/cmsis-dap/short.jpg)



**CRP_DISABLED** drive should show in your computer. Delete the firmware.bin and drag and drop the new [firmware](usbd_hid_dap.bin) file. Reset the board.

![](img/cmsis-dap/crpdisabled.PNG)





### Tutorial



First connect your CMSIS-DAP to MCB1700 over JTAG itnerface.  CMSIS-DAP interface is 



![](img/cmsis-dap/02_jtag_cmsisdap.PNG)



whereas MCB1700 interface is



![](img/cmsis-dap/01_jtag.png)





Hence, the connected boards: 



![](img/cmsis-dap/connected.jpg)





In Keil Uvision you can now choose to program over **JTAG interface**:





![](img/cmsis-dap/jtag.png)





or swd interface:





![](img/cmsis-dap/swd.png)





That's it. You can now compile and load the program:



![](img/cmsis-dap/blinky.PNG)







