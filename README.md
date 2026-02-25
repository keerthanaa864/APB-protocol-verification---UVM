Advanced Peripheral Bus (APB) is the part of Advanced Microcontroller Bus Architecture (AMBA) family protocols. It is a low-cost interface and it is optimized for minimal power consumption and reduced interface complexity.
It is a Non-Pipelined protocol, used to connect low-bandwidth peripherals.

<img width="942" height="327" alt="image" src="https://github.com/user-attachments/assets/71923c0d-76c5-4cac-98e5-eba0be6c7a73" />



Master-Slave communication:


<img width="602" height="360" alt="image" src="https://github.com/user-attachments/assets/161b54fc-6ab2-42a4-98d8-3a0ca6e16d88" />

System bus slave Interface – This is the System bus interface which transfers the AHB/AXI transactions to APB Bridge

PCLK – Generally System clock is directly connected to this

PRESETn – Active Low Asynchronous Reset

PADDR[31:0] – Address bus from Master to Slave, can be up 32 to bit wide

PWDATA[31:0] – Write data bus from Master to Slave, can be up to 32 bit wide

PRDATA[31:0] – Read data us from Slave to Master, can be up to 32 bit wide

PSELx – Slave select signal, there will be one PSEL signal for each slave connected to master.

PENABLE – Indicates the second and subsequent cycles of transfer. 

When PENABLE is asserted, the ACCESS phase in the transfer starts.

PWRITE – Indicates Write when HIGH, Read when LOW.

PREADY – It is used by the slave to include wait states in the transfer.
