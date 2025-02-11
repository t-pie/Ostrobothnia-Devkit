# Ostrobothnia Devkit


## Components
ESP32 + FPGA Integration
-	ESP32 (main controller) → Sends bitstream via SPI, enables wireless updates.
-	iCE40UP5K FPGA → Generates IR pulses, processes received signals.

IR Transmission (Emitter)
-	IR LED (TSAL6200, SFH 4547) for high-speed IR output.
-	MOSFET (BS170, IRLZ34N) to drive the IR LED efficiently.
-	Resistor (~100Ω) to limit current.

IR Reception (Receiver)
-	Photodiode (VBPW34FASR) for fast IR detection.
-	Transimpedance amplifier (OPA354) to amplify the signal.
-	Optional: Phototransistor (TEFT4300) for a simpler alternative.

Debugging & Power
-	SPI Flash (W25Q128) for fast FPGA boot (optional).
-	OLED display / LEDs for status indicators.
-	USB-C for power & programming.
-	JTAG Header (optional) for direct FPGA programming.

## TODO

-  design pcb
-  finish bom
-  ????
-  profit

Link to the Main Repo [Ostrobothnia](https://github.com/t-pie/Ostrobothnia)
