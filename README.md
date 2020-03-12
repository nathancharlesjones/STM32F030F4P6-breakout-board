# STM32F030F4P6 Breakout Board
Image

## MCU specifications
|Part number|Processor|Core Size|Speed|Connectivity|Peripherals|I/O|Program memory size|RAM size|Voltage Supply|Data converters|
|---|---|---|---|---|---|---|---|---|---|---|
|STM32F030F4P6|ARM Cortex-M0|32-bit|48 MHz|I2C, SPI, UART/USART|DMA, POR, PWM, WDT|15|16 kB|4 kB|2.4-3.6V|ADC: 11x 12-bit|

## Schematic
Image

The schematic for this breakout board includes 8 modules or sections:
1. The MCU itself and the 0.1" pin header to which most of the MCU pins are connected (U1 and J1).
2. Power regulator, filtering, and LED indicator (IC1, D1, D2, C1, C2, C3, LED1, and R1).
   - Only C2 and C3 are technically required for MCU operation. If you decide to only include those two components, don't forget to bridge the pads of D1.
   - If IC1 is used, D1 and D2 are strongly recommended (though not technically required). D1 and D2 allow for the MCU to be powered from both the VIN_2.4-3.6V and VIN_5-30V pins at the same time without them damaging each other.
3. The reset button and smoothing capacitor (S1 and C8).
4. BOOT0 selection (J2, R4, and R5): Selects which part of the MCU's memory is run at start-up (see AN for more details).
   - If you intend to use this feature, leave R5 open.
   - If you don't intend to use this feature, use a 0 ohm resistor for R5 to pull BOOT0 to ground.
5. External oscillator (Y1, C6, C7, and R3):
6. Analog voltage reference (D3, C4, and C5):
7. User LED (LED2, R2, and J3):
8. J-Link connector (J4)

### Minimum components


### Standard components

### Full components

## How to order
