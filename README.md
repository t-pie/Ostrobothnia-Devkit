# Ostrobothnia Devkit


## BOM

FPGA + ESP32 Integration
	•	ESP32 (main controller)
	•	Sends bitstream to FPGA via SPI
	•	Handles dynamic configuration
	•	Allows wireless updates via Wi-Fi/Bluetooth
	•	Lattice iCE40UP5K FPGA
	•	Handles precise IR pulse generation
	•	Processes incoming IR signals

IR Transmission (Emitter)
	•	IR LED (TSAL6200, SFH 4547)
	•	High-speed IR LED for transmitting pulses
	•	MOSFET (BS170, IRLZ34N)
	•	Drives IR LED at high speed
	•	Current-limiting resistor (~100Ω)
	•	Protects IR LED

IR Reception (Receiver)
	•	Photodiode (VBPW34FASR, SFH 213 FA)
	•	High-speed IR light detection
	•	Transimpedance amplifier (OPA354, AD8606)
	•	Converts photodiode current to voltage
	•	Optional: Phototransistor (TEFT4300, QSD123)
	•	Simpler, but slightly slower alternative

Debugging & Power
	•	SPI Flash (W25Q128) (for optional fast FPGA boot)
	•	OLED Display (or basic LED indicators)
	•	Show status of FPGA & ESP32
	•	USB-C for power & programming
	•	JTAG Header (for direct FPGA programming)


## TODO

-  design pcb
-  finish bom
-  ????
-  profit

Link to the Main Repo [Ostrobothnia](https://github.com/t-pie/Ostrobothnia)
