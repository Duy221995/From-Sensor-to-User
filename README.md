# Project Report

The auto lighting system

---

## Student information

Student’s name: Nguyen Dinh Duy

Student’s id: ICT20220203

---

**I. Introduction**

The smart decision auto on/off light system is designed to provide an automated lighting solution that adjusts based on the ambient light level. This system aims to improve energy efficiency by automatically turning on the lights when it gets dark and turning them off when it's bright enough. The system utilizes a combination of sensors, data processing techniques, and communication protocols to achieve its functionality.

**II. System Components and Architecture**

1. **System Components:**

a. Light Sensor(ESP32): The system incorporates a light sensor that measures the intensity of ambient light. The sensor provides an analog output that corresponds to the light level in the environment.

b. Microcontroller (Arduino Mega 2560 Rev3): An Arduino microcontroller is used as the main processing unit of the system. It receives the analog output from the light sensor, processes the data, and controls the operation of the LED.

c. LED: An LED serves as the light source that is automatically turned on or off based on the detected light level.

2. **System Architecture:**

The system follows a simple architecture where the light sensor is connected to the microcontroller (Arduino) and the LED. The light sensor provides an analog voltage reading to the microcontroller, which then processes the data and controls the LED's state.

**III. Implementation Details**

3.1 **Explanation of Sensor Selection and Specific Roles:**

In the smart decision auto on/off light system, a light sensor is selected to detect the ambient light level accurately. The specific light sensor used may vary depending on the requirements and available options. Common light sensors such as LDR (Light Dependent Resistor) or photodiodes can be utilized for this purpose. These sensors offer a varying resistance or voltage output based on the intensity of light falling on them. By selecting an appropriate light sensor, the system can effectively measure the light level and make informed decisions.

3.2 **Data Processing Techniques for Informed Decisions:**

The data processing techniques employed in the system involve analyzing the analog output from the light sensor to determine whether the environment is dark or bright. A threshold value is set to distinguish between the two states. If the analog reading falls below the threshold, indicating low light levels, the microcontroller activates the LED by turning it on. Conversely, if the analog reading exceeds the threshold, signifying sufficient light, the microcontroller turns off the LED.

This threshold value can be adjusted based on the specific lighting conditions and sensitivity required for the system. By employing this data processing technique, the system can make intelligent decisions regarding lighting control, ensuring energy efficiency and convenience.

3.3 **Communication Protocols and Technologies for Data Transmission:**

In the context of the smart decision auto on/off light system, communication protocols and technologies are not extensively utilized. The system primarily relies on internal communication between the light sensor, microcontroller, and LED. The light sensor provides an analog output that is directly connected to the microcontroller's analog input pin.

However, if the system is expanded to incorporate additional features, such as remote monitoring or control, communication protocols like UART, SPI, or I2C can be employed. These protocols allow data transmission between the microcontroller and external devices such as a computer or smartphone. This enables remote monitoring of the light sensor readings or the ability to control the light system remotely.

**Conclusion**

The smart decision auto on/off light system provides an energy-efficient and automated lighting solution by utilizing a light sensor, microcontroller, and LED. The system architecture is straightforward, with the microcontroller processing the light sensor's analog output and controlling the LED accordingly. The selection of an appropriate light sensor, data processing techniques, and threshold values ensures that the system can make informed decisions based on the collected data. While the current implementation does not heavily