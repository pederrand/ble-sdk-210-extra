Software handshaking UART
====================

This project is a duplicate of the SimpleNP project in the SDK, and is aimed at adding software handshaking to the NPI protocol on the TI CC2640 BLE SoC. This allows the device to wake up on the UART RX line and enter power saving mode without needing hardware flow control.

This project is built to run on the SmartRF06 Evaluation Board with a CC2650 7x7 Evaluation Module. To use a different board, exchange the Board.c file and change the search path for the board files.

All the files in the project are referenced from their location within the BLE SDK, with the exception of the modified NPI files in this repository: `/Components/npi/**/*swhs.*`

The functionality can be added to an existing project by swapping out the applicable files in your IDE with their `_swhs.*` counterpart, and adding the include search paths.

More information on our wiki:
[http://processors.wiki.ti.com/index.php/NPI Two Wire UART with PM](http://processors.wiki.ti.com/index.php/NPI_Two_Wire_UART_with_PM)
