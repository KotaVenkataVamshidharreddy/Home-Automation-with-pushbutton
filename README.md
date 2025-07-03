# 🏠 Smart Home Automation System

A dual-mode smart home automation system that uses **NodeMCU (ESP8266)** and the **Blynk platform** to control home lighting both manually (via push buttons) and remotely (via smartphone). Designed for real-time responsiveness, ease of use, and scalability toward more IoT devices.

---

## 📸 Demo

| Control Type | Preview |
|--------------|---------|
| Hardware | (![image](https://github.com/user-attachments/assets/47cbd649-a151-4601-8620-8ac02e9e4992)
) |
| Web Control | (![image](https://github.com/user-attachments/assets/82d0b376-a526-412e-a175-cb1b4e86a497)
) |
| Mobile Control | (![image](https://github.com/user-attachments/assets/9a821aba-3a1f-409a-914b-bc087911f275)
) |

---

## 🔧 Project Overview

- **Microcontroller**: NodeMCU ESP8266
- ![image](https://github.com/user-attachments/assets/70126458-310c-4e25-b5a7-871eeea78e3d)


- **Control Modes**: Manual Push Buttons + Blynk Mobile/Web App
- ![image](https://github.com/user-attachments/assets/e7eb4f79-deb0-487b-913c-7cc4d5323ed9)
- ![image](https://github.com/user-attachments/assets/998f9eae-c0ac-45a5-a86b-98467edf0bae)


- **Actuators**: 4-channel Relay Module
- ![image](https://github.com/user-attachments/assets/fc9ac033-5c16-435f-8df8-75f1b7f8adf7)

- **Devices Controlled**: 4 Lights (AC-powered)  
- **Connectivity**: Wi-Fi (Blynk Cloud Integration)  
- **Platform Used**: Arduino IDE
- ![image](https://github.com/user-attachments/assets/bedd5885-22cc-4358-9815-68c49bc4a0c4)


---

## ⚙️ Components Used

| Component            | Description                                 |
|---------------------|---------------------------------------------|
| NodeMCU (ESP8266)   | Central microcontroller with Wi-Fi          |
| 4-Channel Relay     | Switches AC lights                          |
| Push Buttons (x4)   | Manual control for each light               |
| Blynk App & Web     | Remote control via smartphone/web dashboard |
| Power Supply        | 5V input for NodeMCU and relays             |
| AC Bulbs            | Represent lighting appliances               |

---

## 📶 Data Flow
graph TD
A[User sends command from Blynk App/Web] --> B[Blynk Server]
B --> C[NodeMCU receives command via Wi-Fi]
C --> D[Relay toggled via GPIO]
D --> E[Light ON/OFF]
E --> F[Status sent back to Blynk]

![image](https://github.com/user-attachments/assets/91fea95e-248e-424c-8b7d-9682e64beb5e)


## 🔁 Dual-Mode Input

- Push buttons and mobile/web app control
- Real-time feedback to keep app and hardware in sync

---

## 🧠 Features

- Dual control: Remote + Physical  
- Real-time feedback with relay status sync  
- Safe switching of high-voltage lights  
- Expandable for fans, alarms, sensors, etc.  

---

## 🛠️ How to Run

### ⚙️ Hardware Setup

- Connect relay module to NodeMCU GPIO pins (D1–D5)  
- Connect push buttons to D3, D6, D7, RX  
- Wire each light through relay NO/COM pins with AC power  
- Power NodeMCU via USB or 5V adapter  

### 💻 Software Setup

1. Install Arduino IDE and required libraries (`Blynk`, `WiFi`)  
2. Set your Wi-Fi SSID and Blynk Auth Token in code  
3. Upload the code to NodeMCU  
4. Open Serial Monitor to verify connection  
5. Control lights via Blynk app or physical push buttons

---

## 📌 Protocols Used

| Protocol   | Role                                                |
|------------|-----------------------------------------------------|
| Wi-Fi      | Connect NodeMCU to the internet                     |
| HTTP/HTTPS | Communication between Blynk App and Blynk Server    |
| GPIO       | Interface NodeMCU with Relays and Push Buttons      |

---

## ✅ Results

- Successfully toggled 4 AC-powered lights using both app and physical push buttons  
- Real-time feedback ensured app stayed in sync with hardware status  
- Demonstrated reliability, dual-mode control, and smooth user experience  

---

## 📈 Future Scope

- Add motion-based automation using **PIR sensors**  
- Integrate **voice control** using Google Assistant or Alexa  
- Monitor power usage via current/voltage sensors  
- Expand system to control **fans, door locks, alarms**, and other appliances  

---

## 👨‍💻 Contributors

- [Vamshi](https://github.com/KotaVenkataVamshidharreddy/Home-Automation-with-pushbutton.git)  
- Tharun Kumar  
- Surya Teja  
- Rama Krishna Prasad


