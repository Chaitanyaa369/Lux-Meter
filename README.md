💡 Lux Meter with ESP8266

This project is a web-based Lux Meter built using an ESP8266 microcontroller. It measures light intensity using a light sensor and displays the data graphically in real-time through a web interface. The design includes firmware, HTML/JS/CSS for visualization, and a custom-designed PCB.
📦 Project Structure

Lux-Meter/
│
├── Lux_meter/
|   ├── Lux_meter.ino             # Firmware for ESP8266
|   ├── index.html                # Web interface to visualize Lux data
|   ├── style.css                 # Styling for the web interface
│
├── Lux_Meter.sch             # Schematic file (Eagle)
├── Lux_Meter.brd             # PCB layout file (Eagle)
├── LM-Top.pdf                # PCB top view
├── LM-Bottom.pdf             # PCB bottom view
├── LM-C_name_value.pdf       # Component name/value placement
├── LM -components.pdf        # Components and connections
│
└── README.md                 # This file

🧠 Features

    Real-time Lux data visualization using Highcharts

    Simple Start/Stop/Reset buttons for live data streaming

    ESP8266-hosted web server

    Minimal and responsive interface

    Custom PCB design for compact integration

🔧 Hardware Used

    ESP8266 (ESP-12E/F)

    Light sensor (LDR or BH1750)

    LM1117-3.3V voltage regulator

    Capacitors: 100nF, 470pF, 47uF

    Resistors: 12K

    USB-to-Serial interface

    Misc: Connectors, header pins

You can view the hardware setup using:

    📄 LM -components.pdf

    🖼️ LM-Top.pdf and LM-Bottom.pdf

    📐 LM-C_name_value.pdf

💻 Software Used

    Arduino IDE (for programming ESP8266)

    EAGLE CAD (for PCB design)

    HTML/CSS/JavaScript + Highcharts.js (for plotting)

🚀 Getting Started
Flash the Firmware:

    Open Lux_meter.ino in Arduino IDE.

    Install the ESP8266 board support (via Boards Manager).

    Upload the sketch to the ESP8266.

Web Interface:

The ESP8266 serves the index.html and style.css from flash or SPIFFS.

    Open a browser to the ESP8266's IP address.

    The interface provides:

        📈 Real-time chart

        ▶️ Start streaming

        ⏹️ Stop streaming

        🔄 Reset the chart

PCB:

    Open Lux_Meter.sch and Lux_Meter.brd in EAGLE.

    Use the provided PDFs for a quick view of the design and component placement.

🌐 How It Works

    The ESP8266 reads Lux values periodically from the sensor.

    A lightweight web server handles HTTP requests to fetch data.

    The web interface uses JavaScript + Highcharts to plot values dynamically.

📄 License

MIT License. Portions of the web UI adapted from RandomNerdTutorials.
🙏 Acknowledgments

    Rui Santos (Random Nerd Tutorials) for the ESP8266 web interface inspiration

    Highcharts.js for charting library

    Eagle CAD for PCB design

