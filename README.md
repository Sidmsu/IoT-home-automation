# Blynk-Controlled ESP8266

This project demonstrates how to use the ESP8266 WiFi module to connect to the Blynk platform, allowing you to control and monitor your hardware remotely using the Blynk app.

## Components Used

- ESP8266 WiFi Module (e.g., NodeMCU, Wemos D1 Mini)
- USB Cable to connect the ESP8266 to your computer
- Blynk App (available on iOS and Android)
- WiFi Network

## Features

- **Remote Control**: Use the Blynk app to control the ESP8266 over WiFi.
- **Real-Time Monitoring**: Monitor sensor data and other parameters in real-time.
- **Easy Setup**: Connect to Blynk using simple authentication.

## Setup and Installation

### Prerequisites

- Arduino IDE installed on your computer
- Blynk app installed on your smartphone
- A Blynk account (create one in the app)


1. **Install Blynk Library:**

    Open Arduino IDE and go to `Sketch > Include Library > Manage Libraries`. Search for "Blynk" and install the Blynk library.

2. **Configure WiFi and Blynk Auth Token:**

    - Open the `Blynk_Controlled_ESP8266.ino` file in the Arduino IDE.
    - Replace `"YourAuthToken"` with the Auth Token you received from the Blynk app.
    - Replace `"YourNetworkName"` with your WiFi network name.
    - Replace `"YourPassword"` with your WiFi password.

3. **Upload the Code:**

    - Connect your ESP8266 to your computer via USB.
    - Select the correct board and port in the Arduino IDE (`Tools > Board > NodeMCU 1.0` and `Tools > Port`).
    - Click the Upload button.



### Key Components

- **WiFi Connection**: The ESP8266 connects to your WiFi network using the provided SSID and password.
- **Blynk Connection**: Uses the Blynk library to connect to the Blynk server with your Auth Token.
- **Main Loop**: Continuously runs the Blynk process to maintain the connection and handle events.

## How to Use

1. **Set Up Blynk App:**
    - Open the Blynk app and create a new project.
    - Add widgets (e.g., buttons, sliders) to control or monitor your ESP8266.
    - Get the Auth Token from the project settings and insert it into the code.

2. **Run the ESP8266:**
    - After uploading the code, open the Serial Monitor in Arduino IDE to check the connection status.
    - The ESP8266 will connect to your WiFi network and then to the Blynk server.

3. **Control and Monitor:**
    - Use the Blynk app to send commands to the ESP8266 or monitor sensor data.

## Troubleshooting

- **Connection Issues**: Ensure your SSID and password are correct. Check the Serial Monitor for error messages.
- **Auth Token**: Make sure the Auth Token in the code matches the one provided by the Blynk app.

## Contributing

Contributions are welcome! Feel free to fork this repository and submit pull requests.


## Acknowledgments

- Blynk for providing the platform and library
- Arduino community for the resources and support

