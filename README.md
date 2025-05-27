# 📦 Time-Based Priority Dispatch System for Warehouses Using Low-Cost Embedded Hardware


![WhatsApp Image 2025-05-25 at 17 35 20_f5c371ae](https://github.com/user-attachments/assets/aaeac862-72fd-4175-b29e-24ea10ddaa1e)




A real-time warehouse dispatch automation system using **ESP32**, **RFID**, and **Google Firebase**, designed for small and medium-scale warehouses. This project focuses on intelligent, low-cost automation for efficient, priority-based dispatch operations.

---

## 🚀 Project Overview

- Real-time product tracking
- Priority classification based on delivery urgency
- Automated zone allocation
- Dispatch monitoring via a web dashboard

Incoming products are scanned via RFID, categorized by delivery time, and stored in different zones (Zone 1 → Zone 3). As dispatch time approaches, the product is automatically flagged, tracked, and logged in Firebase.

---

## 🧠 Features

✅ RFID-based product scanning  
✅ Real-Time Clock (RTC) for delivery countdown  
✅ ESP32 Wi-Fi sync with Firebase  
✅ Dynamic zone-block allocation  
✅ Real-time React + Firebase dashboard  
✅ Product classification (High, Medium, Low Priority)  
✅ Dispatch history tracking  

---

## 📦 Warehouse Layout


![WhatsApp Image 2025-05-25 at 17 35 21_a7a2ebd0](https://github.com/user-attachments/assets/8c4e63f3-1e78-44e2-82bc-9362bca5f2bc)


| Zone   | Priority        | Time Frame         |
|--------|------------------|--------------------|
| Zone 3 | High Priority    | Delivery ≤ 24 hrs  |
| Zone 2 | Medium Priority  | Delivery ≤ 3 days  |
| Zone 1 | Low Priority     | Delivery > 3 days  |

Each zone contains **Blocks A, B, C** for organized product storage.

---

## 🛠️ Hardware Used

| Component        | Description                 | Cost (INR) |
|------------------|-----------------------------|------------|
| ESP32 Dev Board  | Wi-Fi microcontroller        | ₹300       |
| RFID RC522       | RFID Reader Module           | ₹150       |
| RFID Tags        | Passive RFID Tags (10 qty)   | ₹200       |
| RTC Module       | Real-Time Clock Module       | ₹100       |
| Power Adapter    | 5V DC                        | ₹150       |
| Misc Components  | Wires, PCB, breadboard       | ₹200       |
| **Total**        |                             | **₹1,000** |

---

## 💻 Software Stack

- **Arduino IDE** – ESP32 Programming
- **Google Firebase** – Real-time Cloud Database
- **React.js** – Web dashboard frontend
- **Node.js** – Backend logic (if needed)
- **Firebase Hosting** (optional)

---

## 📊 Web Dashboard


![WhatsApp Image 2025-05-25 at 17 35 22_f39c05a1](https://github.com/user-attachments/assets/a0447d27-faeb-491c-95b1-dfff522bd9c5)


- Track total, dispatched, and pending products
- View products by zone and block
- See delivery deadlines and customer info
- Realtime dispatch log with status updates

---

## 🔁 Dispatch Logic

1. Product scanned via RFID on arrival
2. ESP32 sends data to Firebase
3. Delivery time evaluated → Zone/Block assigned
4. RTC tracks dispatch time
5. Dashboard updated in real-time
6. Final scan marks product as "Dispatched"

---

## 📚 Documentation

You can find the full research paper in Above Files

---

## 📦 Use Cases

- Small to medium warehouse operations
- Educational warehouse automation prototypes
- Real-time inventory & logistics systems

---

## 🔮 Future Scope

- Integration with robotic conveyors
- Mobile app interface with Firebase
- Offline caching with sync
- AI-based product movement optimization

---
