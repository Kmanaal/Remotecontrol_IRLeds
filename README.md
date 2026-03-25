# Remotecontrol_IRLeds

# WORKING PRINCIPLE

Remote-controlled LED is pretty self-explanatory. The IR-controlled LED system operates by
using modulated IR signals to transmit commands from a remote control to an LED circuit. The
IR signals are detected, demodulated, and decoded by the receiver on the LED circuit, leading to
the execution of specific commands to control the LED's state.

The working principle of the project is as follows:

## 1. Transmitter (Remote Control):
• IR LED Emission: The remote control contains an Infrared LED that emits modulated
IR signals when a button is pressed. The IR LED modulates the infrared light to
encode information. Each button on the remote control is associated with a specific
binary code or sequence of pulses, encoding a particular command.

## 2. Receiver (IR Sensor on LED Circuit):
• IR Receiver: The LED circuit includes an IR receiver that is sensitive to infrared light.
The IR receiver constantly listens for incoming IR signals. When an IR signal is
detected, the receiver demodulates the signal, extracting the encoded information.
• Command Interpretation: The demodulated signal is received and fed into Arduino
via pin “2”. Where it interprets the command.

## 3. LED Control:
• Command Execution: Based on the decoded information, the microcontroller
executes the corresponding command. The LED state is controlled accordingly. LEDs
are connected to pin “8,9,10,11” of Arduino

# MODULATION / DEMODULATION
In infrared (IR) remote controls, the most common modulation/demodulation technique is
Amplitude Shift Keying (ASK). The remote control transmits the modulated signal whereas this
project demodulates and decodes the information.

## ASK (Amplitude Shift Keying) MODULATION:
ASK is a simple and widely used modulation method that encodes
information by varying the amplitude of the carrier signal. It is a type ofAmplitude Modulation
that represents the binary data in the form of variations in the amplitude of a signal.

Any modulated signal has a high-frequency carrier. The binary signal
when ASK modulated, gives a zero value for Low input while it gives the carrier output for High
input.

In the context of IR remote controls, here's how ASK modulation works:

### 1. Continuous Wave (CW) Modulation:
• The IR LED in the remote control continuously emits infrared light in the form of a continuous wave.

### 2. Binary Encoding:
• Each button press on the remote control corresponds to a specific binary code. The binary code is encoded and transmitted by modulating the amplitude of the IR signal following the protocol used by the remote control.
