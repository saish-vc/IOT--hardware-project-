# 💡 ESP32 Smart Light Control System

> A beginner-friendly IoT project to control an LED (and later real appliances) over Wi-Fi using an ESP32 microcontroller and a browser-based interface.

---

## 🎯 Project Goal

Build a system where your phone or laptop can control an LED over Wi-Fi — laying the foundation for a full smart home setup.

```
Phone / Laptop
      ↓  Wi-Fi
    ESP32
      ↓
  LED ON/OFF
```

> **Later, the same logic scales to:** real bulbs, fans, relays, and Home Assistant integration.

---

## ✅ What You'll Build

- Program an ESP32 microcontroller
- Connect it to your home Wi-Fi
- Host a web server directly on the ESP32
- Control an LED from any browser on the same network

**Example:**
```
http://192.168.1.5/on   →  LED turns ON
http://192.168.1.5/off  →  LED turns OFF
```

---

## 🛒 Components & Budget

| Item | Approx. Price (INR) |
|------|-------------------|
| ESP32 Dev Board | ₹500 – ₹700 |
| Breadboard | ₹100 |
| Jumper Wires | ₹100 |
| LED | ₹10 |
| Resistor (220Ω – 330Ω) | ₹10 |
| USB Cable | Usually included |
| **Total** | **~₹800 – ₹1000** |

---

## 🔩 Components Explained

### 1. ESP32
A microcontroller with built-in **Wi-Fi**, **Bluetooth**, and **GPIO pins**.  
Think of it as a tiny programmable computer for electronics.

### 2. Breadboard
Lets you connect components without soldering — perfect for prototyping.

### 3. Jumper Wires
Connect pins between the ESP32 and other components on the breadboard.

### 4. LED
Represents your appliance in this phase.  
Upgrade path: `LED → Relay → Real Appliance`

### 5. Resistor (220Ω – 330Ω)
Protects the LED from excessive current draw.

---

## 🏗️ System Architecture

```
Browser
   ↓
Wi-Fi Router
   ↓
ESP32 Web Server
   ↓
GPIO Pin
   ↓
LED
```

### How It Works

| Step | Action |
|------|--------|
| 1 | ESP32 connects to your home Wi-Fi |
| 2 | ESP32 starts a mini web server (e.g., `http://192.168.1.5`) |
| 3 | Browser sends a request (`/LED=ON`) |
| 4 | ESP32 sets the GPIO pin HIGH |
| 5 | LED turns ON |

---

## 🗓️ 6-Week Roadmap

### Week 1 — Learn the Basics
- What is the ESP32?
- GPIO pins: input vs output
- Voltage basics (3.3V, 5V, GND)
- Watch ESP32 introduction and basic electronics tutorials

### Week 2 — Setup Development Environment
- Install [Arduino IDE](https://www.arduino.cc/en/software)
- Install the ESP32 board package via Board Manager
- Verify you can upload a sketch

### Week 3 — Blink an LED
- Write your first program: make an LED blink
- Learn GPIO output control
- Practice uploading code and debugging

### Week 4 — Connect to Wi-Fi
- Connect the ESP32 to your home network
- Understand SSIDs, IP addresses, and routers
- Print the assigned IP to Serial Monitor

### Week 5 — Create a Web Server
- Host a basic webpage from the ESP32
- Open `http://<ESP32_IP>` in your browser
- Serve a simple HTML response

### Week 6 — Browser-Controlled LED
- Add ON and OFF buttons to the webpage
- Handle HTTP requests on the ESP32
- Toggle the LED remotely from any device on your network

---

## 🏁 Final Result

By the end of Phase 1, you will have:

- ✅ A Wi-Fi connected ESP32
- ✅ A browser-controlled device
- ✅ A solid IoT foundation
- ✅ A working smart device — ready to scale

---

## 🚀 What's Next? (Phase 2 Preview)

- Replace the LED with a **relay module**
- Control **real appliances** (lamps, fans)
- Add a **mobile-friendly UI**
- Integrate with **Home Assistant** or **MQTT**
- Add **schedules and automation logic**

---

## 📚 Resources

- [ESP32 Official Docs](https://docs.espressif.com/projects/esp-idf/en/latest/)
- [Arduino IDE Download](https://www.arduino.cc/en/software)
- [ESP32 Arduino Core (GitHub)](https://github.com/espressif/arduino-esp32)
- [Random Nerd Tutorials — ESP32](https://randomnerdtutorials.com/projects-esp32/)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

*Happy building! 🔧⚡*
