## uC/OS-II port for Microsemi RISC-V

### Test Platform and FPGA design:
M2GL025-Creative-Board
[M2GL025-Creative Board RISC-V Sample Design](https://github.com/RISCV-on-Microsemi-FPGA/M2GL025-Creative-Board/tree/master/Modify_The_FPGA_Design/CoreRISCV_AXI4_BaseDesign)    

### How to run the uC/OS-II RISC-V port:
To know how to use the SoftConsole workspace, please refer the [Readme.md](https://github.com/RISCV-on-Microsemi-FPGA/SoftConsole/blob/master/ExampleWorkspace/README.md)

Top folders of riscv-uCOS-sample

`bsp`: Board Support Package source code for LED's and OS Tick timer

`drivers`: This folder contains DirectCore Soft IP CoreGPIO and CoreUARTapb drivers source code.

`hal and riscv_hal`: This folder provides RISC-V soft processor hardware abstraction layer(RISC-V HAL) boot code, interrupt handling and hardware access methods for RISC-V soft processor. The source code also downloadable from GitHub [RISCV-on-Microsemi-FPGA](https://github.com/RISCV-on-Microsemi-FPGA/riscv-hal)

`Micrium`: uC/OS-II for RISC-V port source code
    
`Micrium_libgen`: This Folder contains library file of uC/OS-II. The application can call OS services(FLAGS, Mailboxes, Mutex, SoftwareTimer, semaphores.. etc) using this library and also find the API of uC/OS-II in documentation at [micrium website](https://doc.micrium.com/pages/viewpage.action?pageId=16879190)    


The riscv-uCOS-sample is a self contained project. This project demonstrates 
the uC/OS-II running with Microsemi RISC-V processor. This project creates  three 
tasks and runs them at regular intervals.
    
This example project requires USB-UART interface to be connected to a host PC. 
The host PC must connect to the serial port using a terminal emulator such as 
TeraTerm or PuTTY configured as follows:
    
        - 115200 baud
        - 8 data bits
        - 1 stop bit
        - no parity
        - no flow control
    
The ./hw_platform.h file contains the design related information that is required 
for this project. If you update the design, the hw_platform.h must be updated 
accordingly.
    
### Microsemi SoftConsole Toolchain:
To know more please refer: [SoftConsole](https://github.com/RISCV-on-Microsemi-FPGA/SoftConsole)

### Documentation for Microsemi RISC-V processor, SoftConsole toochain, Debug Tools, FPGA design etc.
To know more please refer: [Documentation](https://github.com/RISCV-on-Microsemi-FPGA/Documentation)
    
