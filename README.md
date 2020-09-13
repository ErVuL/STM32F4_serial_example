# STM32F4_serial_example

USB Serial Communication with PC.
Return the entered char throughout the serial virtual port.

Modifications done in:
usbd_cdc_if.c ==> static int8_t CDC_Receive_FS(uint8_t* Buf, uint32_t *Len)

Baudrate = 115200
