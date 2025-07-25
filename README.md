# TEMPERATURE-MONITORING-SYSTEM

**COMPANY**: CODTECH IT SOLUTIONS

**NAME**: RIFANA NAZREEN A

**INTERN ID**:CT04DH23

**DOMAIN**: EMBEDDED SYSTEMS

**DURATION**: 4 WEEKS

**MENTOR**: NEELA SANTHOSH

DESCRIPTION:

This project is a temperature monitoring system using an Arduino Uno, an LM35 temperature sensor, and a 16x2 LCD display. It reads the temperature in Celsius and shows it on both the LCD and the serial monitor.

In the circuit, the LM35 sensor is placed on a breadboard. It has three pins: VCC, GND, and output. The output pin is connected to analog pin A0 of the Arduino. The sensor gives an analog voltage proportional to temperature.

The LCD is connected in 4-bit mode to digital pins 12, 11, 5, 4, 3, and 2. A potentiometer is used to adjust the LCD contrast. One side of the potentiometer is connected to 5V, the other to GND, and the middle pin goes to the LCD's V0 pin.

In the code, the analog value from the temperature sensor is read using `analogRead(tempPin)`. This value is converted to voltage using the formula `voltage = sensorValue * (5.0 / 1023.0)`. The voltage is then converted to temperature using the formula `temperatureC = (voltage - 0.5) * 100.0`, which is specific for the LM35 sensor.

The LCD is initialized in the setup section, and a welcome message is displayed briefly. In the loop, the temperature is continuously read and displayed on both the LCD and serial monitor every second.

This setup can be used in projects requiring simple temperature tracking, such as room monitoring or weather stations.

OUTPUT:

<img width="1207" height="718" alt="Image" src="https://github.com/user-attachments/assets/efed754d-dd7e-4719-9108-6ee651cd6413" />
