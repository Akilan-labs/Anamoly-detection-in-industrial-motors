 Anomaly Detection in Industrial Motors using Edge AI & STM32
This project focuses on using Edge AI to detect faults in industrial motors in real time. By deploying lightweight machine learning models on STM32 microcontrollers, we can identify unusual behavior such as abnormal vibrations or overheating — helping prevent unexpected failures and reduce downtime on the factory floor.

What This Project Does
Monitors motors for signs of trouble like vibration spikes or unusual temperature changes

Uses AI models trained on real sensor data to catch issues early

Runs entirely on a microcontroller (no cloud or PC needed)

Sends alerts when something doesn’t look right

 What’s Under the Hood
 Hardware: STM32 boards (e.g., STM32F411, STM32L432KC)

 ML Framework: TensorFlow Lite for Microcontrollers

 Development Tools: STM32Cube.AI, STM32CubeIDE

 Sensors Used: Vibration (MPU6050), temperature, and motor current

Training Code: Python with TensorFlow or scikit-learn

Optional Communication: UART, USB, Bluetooth, or MQTT

How It All Works
Collect Data
Gather sensor readings from motors in both normal and faulty conditions.

Preprocess the Data
Filter noise, normalize values, and prepare datasets for training.

Train the Model
Use techniques like autoencoders or classifiers to recognize what "normal" looks like.

Convert the Model
Turn it into a .tflite version optimized for microcontrollers using STM32Cube.AI.

Deploy to the Board
Flash the model and code onto an STM32 using STM32CubeIDE.

Run in Real-Time
The board continuously reads live data, runs predictions, and raises alerts on anomalies.
