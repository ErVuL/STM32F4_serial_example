# STM32F4_serial_example

USB Serial Communication between PC and STM32F407VG.
STM32CubeIDE 1.4.0 project.

It return the entered char throughout the serial virtual port.

Modifications done in:
usbd_cdc_if.c ==> static int8_t CDC_Receive_FS(uint8_t* Buf, uint32_t *Len)

Serial COM proprieties (PuTTY):
+ Baudrate = 115200
+ data bits = 1 byte
+ stop bits = 1
+ parity = none
+ Flow control: XON/XOFF

TODO:
      + Add interrupt to get the UserRxBufferFS data into the main() function.
          --> How to use semaphore/mutex/atomic or __HAL_LOCK() ?
