## uC/OS-II port for Microsemi RISC-V

### Test Platform and FPGA design:
MPF300T-PolarFire-Eval-Kit
[PolarFire Evaluation Kit RISC-V Sample Design](https://github.com/RISCV-on-Microsemi-FPGA/MPF300T-PolarFire-Eval-Kit/tree/master/Modify_The_FPGA_Design/PF_CoreRISCV_AXI4_BaseDesign)    

### How to run the uC/OS-II RISC-V port:
To know how to use the SoftConsole workspace, please refer the [Readme.md](https://github.com/RISCV-on-Microsemi-FPGA/SoftConsole/blob/master/ExampleWorkspace/README.md)

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
    
