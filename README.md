# Arduino--Adafruit-Data-Transfer

This project deals with data logging of voltage values of an LED using a potentiometer. The components used are 

1. Node MCU ESP8266
2. LED
3. 10K Potentiometer
4. 1K Resistor

We have made use of Adafriut Cloud Service. For information about Adafruit, refer [https://www.adafruit.com/about](https://www.adafruit.com/about).

The circuit was setup as shown in the figure. 

<p align="center"><img src="https://user-images.githubusercontent.com/48091500/59160096-5aff2c00-8aef-11e9-9f75-de4a5d61d5ed.jpg" height="450"></p>
  
### <p align="center">Fig 1. Circuit Showing the Connections</p>

The two fixed ends of the potentiometer were connected to 3V supply and GND(Ground). The variable end was connected to an analog pin(A0) of the MCU. The ADC pin has a 10-bit resolution, which means you'll get values between 0 and 1023. These values were converted to voltage values. The LED was connected to the digital pin(D0) of the MCU. This was done to show physically the working of the circuit As the potentiometer knob was varied, the LED luminosity varied and the voltage values across the potentiometer were sent over to the Cloud Service via Wi-Fi. These values were displayed on a graph as shown in figure.

<p align="center"><img src="https://user-images.githubusercontent.com/48091500/59159687-15406480-8aeb-11e9-8576-b7075897cd7f.JPG" alt="AdafruitIO_Potentiometer_Voltage" width="750" height="350" /></p>

### <p align="center">Fig 2. Plotting of Graph for Different Voltage Values where Y-axis is Voltage(V) and X-axix is Time(h:min:s)</p>

For more information on ESP8266, refer [ESP8266 Datasheet](https://www.espressif.com/sites/default/files/documentation/0a-esp8266ex_datasheet_en.pdf).
