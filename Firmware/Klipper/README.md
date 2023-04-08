* `Building the micro-controller` with the configuration shown below. (If your klipper cannot select the following configuration, please update your klipper source code)
    * [*] Enable extra low-level configuration options
    * Micro-controller Architecture = `STMicroelectronics STM32`
    * Processor model = `STM32G0B1`
    * Bootloader offset = `8KiB bootloader`
    * Clock Reference = `8 MHz crystal`
    * IF USE USB
        * Communication interface = `USB (on PA11/PA12)`
    * ElSE IF USE CANBUS
        * Communication interface = `(CAN bus (on PD0/PD1))`
    * ELSE IF USE USB to CAN bus bridge
        * Communication interface = `USB to CAN bus bridge (USB on PA11/PA12)`
        * CAN bus interface = `CAN bus (on PD0/PD1)`
    * (PA4) GPIO pins to set at micro-controller startup

    <img src=menuconfig.png width="800" /><br/>