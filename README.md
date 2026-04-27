# Bridge-soil-sensor-irrigation-27-4-2026
# 🌱 Irrigation System Project

## 📌 Overview

This project focuses on designing and implementing an efficient irrigation system using simple technology. The goal is to optimize water usage, improve crop growth, and reduce manual effort by automating the watering process.

## ⚙️ Features

* Automatic watering based on soil moisture levels
* Water-saving irrigation method
* Easy to build and low-cost components
* Can be implemented using microcontrollers (e.g., Arduino)
* Suitable for farms, gardens, and greenhouses

## 🧰 Components Used

* Soil Moisture Sensor
* Microcontroller (Arduino Uno / Mega)
* Water Pump
* Relay Module
* Connecting Wires
* Power Supply
* Water Pipes / Tubing

## 🔌 System Working

1. The soil moisture sensor detects the level of moisture in the soil.
2. The sensor sends data to the microcontroller.
3. If the soil is dry, the microcontroller activates the relay.
4. The relay turns on the water pump.
5. Water is supplied to the plants automatically.
6. Once sufficient moisture is reached, the system turns off the pump.

## 🖼️ Diagram

*(You can add your Tinkercad or circuit diagram image here)*

## 💻 Sample Code

```cpp
int sensorPin = A0;
int pumpPin = 7;
int moistureValue;

void setup() {
  pinMode(pumpPin, OUTPUT);
  Serial.begin(9600);
}

void loop() {
  moistureValue = analogRead(sensorPin);
  Serial.println(moistureValue);

  if (moistureValue < 500) {
    digitalWrite(pumpPin, HIGH); // Pump ON
  } else {
    digitalWrite(pumpPin, LOW);  // Pump OFF
  }

  delay(1000);
}
```

## 🚀 How to Use

1. Connect all components as shown in the diagram.
2. Upload the code to your Arduino board.
3. Place the sensor in the soil.
4. Power the system.
5. The irrigation system will work automatically.

## 📈 Advantages

* Saves water
* Reduces human effort
* Improves plant health
* Low maintenance

## ⚠️ Limitations

* Requires power supply
* Sensor accuracy may vary
* Needs proper setup and calibration

## 🔮 Future Improvements

* Add IoT for remote monitoring
* Use solar power for energy efficiency
* Mobile app control
* Weather-based irrigation system

## 👨‍💻 Author

* Your Name

## 📄 License

This project is open-source and free to use for educational purposes.

---

💧 *Smart irrigation leads to smarter farming!*
