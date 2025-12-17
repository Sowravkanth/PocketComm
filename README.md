# ⚡ PocketComm

> **Unbreakable Connection When Grids Fail.**

**PocketComm** is a tactical, infrastructure-independent communication ecosystem engineered for "Last Mile" connectivity during catastrophic network failures. By orchestrating a hybrid architecture of **Bluetooth**, **LoRa (Long Range)**, and **Cloud Computing**, PocketComm transforms a simple smartphone into a life-saving satellite-alternative for disaster management and remote exploration.

---

## 🚀 The Mission: Beyond the Last Mile

In a country as geographically diverse as India, cellular networks are the first casualty of floods, cyclones, and earthquakes. PocketComm addresses this "Zero Communication" crisis by delivering:

* **Disaster-Proof Messaging**: Free-text emergency communication across kilometers without relying on telecom towers or SIM cards.


* **Guaranteed Reliability**: A custom acknowledgement-based protocol ensures your distress signal is heard and logged.


* **AI-Prioritized Rescue**: Integration with **Google Gemini AI** to automatically classify and rank incoming alerts based on medical urgency.



---

## 🛠️ System Architecture & Components

PocketComm utilizes a **Hybrid Edge-Cloud Topology** to ensure data survives the air-gap.

### **Hardware Manifest (BOM)**

| Component | Specification | Role |
| --- | --- | --- |
| **MCU** | ESP32 | Dual-core processing (240MHz) for multitasking.|
| **Radio** | SX1278 LoRa (433MHz) | Long-range penetration using Spread Spectrum Modulation.|
| **Navigator** | NEO-6M GPS | Atomic-clock precision for geolocation tagging.|
| **Display** | 0.96" SSD1306 OLED | Heads-Up Display (HUD) for real-time status feedback. |

### **Software Stack**

* **Embedded Layer**: C++ / Arduino IDE for node firmware.

* **Communication Layer**: Bluetooth Classic (Smartphone to ESP32) and LoRa RF (Node to Node).

* **Cloud & Backend**: Firebase Realtime Database for sub-second synchronization.

* **Intelligence Layer**: Google Gemini API for message classification and priority scoring.

* **Interface**: Tactical Web Dashboard (HTML, CSS, JS).


---

## ⚙️ Core Innovations

* **"Smart-Lock" Telemetry**: Every message is automatically stamped with real-time GPS coordinates at the sender node.

* **Dynamic Information Display**: A custom software routine that manages real-time status updates on the OLED screen.
  
* **No-App Interface**: Users connect via standard Bluetooth Terminal apps—no proprietary software downloads required during an emergency.


* **Infrastructure Independence**: Operates completely independent of telecom infrastructure during disasters.



---

## 📊 Sample Outputs

### **1. Base Station (Receiver) Serial Monitor**

```text
=== POCKETCOMM BASE STATION ONLINE ===
[NET] Uplink Secured. IP: 192.168.1.104
[RAD] Radio Listening on 433MHz (Sync: 0xF3)

┌──────────────────────────────────────────────────┐
│ INCOMING PACKET DETECTED | T+45200ms             
├──────────────────────────────────────────────────┤
│ [SIGNAL] RSSI: -48 dBm  | SNR: 9.25              
│ [SOURCE] ID  : ALPHA-01                          
│ [STATUS] BAT : 98%                               
├──────────────────────────────────────────────────┤
│ [PAYLOAD] Medical Emergency, Send Help!          
│ [GEO-LOC] 12.9716, 77.5946                        
└──────────────────────────────────────────────────┘
[CLOUD] Syncing to Command Center... DONE.

```

### **2. Handheld (Sender) OLED HUD**

```text
-------------------
BT:ON    SAT:08   98%    <-- System Health Bar
-------------------

      ARMED              <-- System Status

   Ready to Send         <-- Operation Mode

```

---

Team PowerHouse 

* S. Sowravkanth**


* **Y.Hrithik**


* **Tejeshwar A.S**


* **Tharun Raj A.M**
 

* **Muthukumaran.T**


* **Hemanth A.R**



---

## 📄 License

This project is open-source and available under the [MIT License](https://www.google.com/search?q=LICENSE).

> **PocketComm: Communication Without Boundaries.**
