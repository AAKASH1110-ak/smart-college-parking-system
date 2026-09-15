# AI-Powered Smart College Parking Management System 🚗⚡

**Student Details:**
- **Name:** Aakash RB
- **Department:** Computer Science and Engineering (CSE)
- **Institution:** Rathinam Technical Campus
- **Batch:** 2025–2029
- **Project Domain:** Smart Campus Mobility / AI Immersion & Design Thinking

---

## 📌 1. Project Overview & Goal
College campuses experience severe vehicular congestion during morning peak hours (8:45 AM – 9:30 AM), resulting in students and faculty circling parking bays, late arrivals to lectures and labs, fuel wastage, and hazardous double parking.

The **AI-Powered Smart College Parking Management System** solves this campus bottleneck by:
1. Predicting lot availability ahead of time using historical schedule curves.
2. Recommending the optimal parking zone and slot based on the driver’s destination academic block (e.g. CSE Block).
3. Providing contactless, paperless QR gate clearance with boom-barrier automation.
4. Equipping campus administrators with real-time zone telemetry, dynamic traffic rerouting, and simulated AI anomaly insights.

---

## 🏛️ 2. System Architecture

```
┌─────────────────────────────────────────────────────────────────────────────┐
│             AI-Powered Smart College Parking Management System              │
│       Rathinam Technical Campus • CSE Dept • Aakash RB (2025–2029)          │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│  [Top Bar / Role Switcher / Demo Controls: Normal | Rush Hour | Zone A Full]│
│                                                                             │
│  ┌───────────────────────────┬───────────────────────────────────────────┐  │
│  │ Navigation Tabs           │ Active View / Interactive Screens        │  │
│  ├───────────────────────────┼───────────────────────────────────────────┤  │
│  │ 1. Home / Landing Page    │ • Hero "Park Smarter. Arrive Faster."     │  │
│  │ 2. Student Dashboard      │ • "Good morning, Aakash 👋" + Quick Stats │  │
│  │ 3. Live Campus Map        │ • Zones A-E with Live Color-Coded Heatmap │  │
│  │ 4. Slot Matrix Explorer   │ • A-01..A-50, EV, Two-Wheeler, Accessible │  │
│  │ 5. AI Best Parking Finder │ • Distance/Walk-Time/Congestion Recommender│ │
│  │ 6. AI Predictive Forecast │ • 8 AM - 12 PM Demand Curves & Best Time  │  │
│  │ 7. Book Reservation       │ • Booking Form + Digital Pass + QR Code   │  │
│  │ 8. Gate QR Scanner Sim    │ • Boom-barrier Entry & Exit Gate Animator │  │
│  │ 9. My Vehicles Fleet      │ • Vehicle Registry (Car/Bike/EV/Color)   │  │
│  │ 10. Parking History       │ • Audit log of past check-ins & duration  │  │
│  │ 11. Report Issue          │ • Blocked slot, EV charger fault ticket   │  │
│  │ 12. Admin AI Dashboard    │ • 500 Total, 312 Occ, Insights & Reroute  │  │
│  └───────────────────────────┴───────────────────────────────────────────┘  │
│                                                                             │
│  [Floating Components: ParkAI Chatbot Assistant + Instant Notification Bell]│
└─────────────────────────────────────────────────────────────────────────────┘
```

The system is built on a **Component-Driven Modular Architecture**:
- **Presentation Layer:** React 18 + TypeScript + Tailwind CSS with dark navy glassmorphism.
- **State Management & Logic:** Centralized `ParkingContext` providing dynamic synchronization between slots, reservations, vehicle profiles, notifications, and demo modes.
- **Simulation Engines:**
  - **AI Time-Series Forecaster:** Models hourly occupancy from 8:00 AM to 12:00 PM.
  - **AI Multi-Criteria Decision Matrix (MCDM):** Evaluates walking distance, lane congestion, and slot category to recommend spots like `Zone A, Slot A-12`.
  - **ANPR & IoT Barrier Simulator:** Simulates camera OCR plate scanning and servo boom-barrier arm movement with Web Audio feedback.
  - **ParkAI Chatbot Engine:** Floating natural language assistant answering campus parking queries.

---

## 🖥️ 3. Main Pages & Interactive Views

| View / Page | Key Functionality |
| :--- | :--- |
| **Landing Page** | High-impact hero: *"Park Smarter. Arrive Faster."*, problem vs AI solution breakdown, key metrics ribbon, quick-action CTAs. |
| **Student Dashboard** | Personalized greeting: *"Good morning, Aakash 👋"*, real-time counters (Available, Occupied, Reserved), nearest zone (Zone A, 120m), AI recommended spot, active reservation widget with QR pass trigger, live alert notices. |
| **Live Campus Map** | SVG architectural layout of Rathinam Technical Campus featuring Academic Blocks (CSE, Library, Admin, Cafeteria, Mech) and 5 Zones (A: 50, B: 40, C: 60, D: 80, E: 30) with dynamic status colors (🟢 Green, 🟡 Yellow, 🔴 Red, 🔵 Blue). |
| **Slot Grid Explorer** | High-density slot matrix (e.g. A-01 to A-50) filterable by slot type: Standard Car, Two-Wheeler / Bike, EV Fast Charging, Accessible (Divyangjan), and Visitor. |
| **AI "Find Best Parking"** | Multi-criteria recommendation tool where students input their destination building (e.g. CSE Block) and vehicle type to calculate optimal spot, walking distance, and time. |
| **AI Hourly Forecast** | Simulated time-series occupancy curve charting 8:00 AM (72%), 9:00 AM (48%), 10:00 AM (31% peak rush), 11:00 AM (55%), and 12:00 PM (68%). |
| **QR Gate Scanner** | Dual-mode boom-barrier terminal simulator (Campus Entry vs Exit) with animated barrier arm, laser scanner effect, OCR plate verification, and sound chime. |
| **My Vehicles Fleet** | Manage student vehicle profiles (Ather 450X, Hyundai i20, Hunter 350) with default vehicle toggling and registration modal. |
| **Parking History** | Searchable audit trail of past campus check-ins with entry/exit timestamps, total duration, and export to CSV simulation. |
| **EV & Accessible** | Dedicated view showcasing 22kW/7.4kW Type 2 EV chargers, solar grid canopy status, and zero-step ramp routes for accessible parking. |
| **Admin AI Dashboard** | High-level campus overview with official stats: 500 total spaces, 312 occupied, 188 available, 42 reserved, 1,284 today's vehicles, zone capacity bars, peak-hour ingress analytics, and emergency barrier release controls. |

---

## 🚀 4. Implemented Features (18 / 18 Complete)

1. ✅ **Landing Page:** Hero “Park Smarter. Arrive Faster.”, problem & solution cards, “Find Parking” & “View Parking Map” CTAs.
2. ✅ **Login / Signup:** Multi-persona mock auth (Student Aakash RB, Faculty Dr. Mohan, Staff Saravanan, Visitor Karthik, Admin).
3. ✅ **Student Dashboard:** Personalized “Good morning, Aakash 👋” greeting, CSE block badge, live metrics, walk distance/time.
4. ✅ **Live Parking Map:** Interactive SVG map featuring Zones A (50), B (40), C (60), D (80), E (30) with status colors: Green, Yellow, Red, Blue.
5. ✅ **Individual Parking Slots:** Interactive slot cards (A-01, A-02...) categorized by Car, Two-wheeler, EV, Accessible, and Visitor.
6. ✅ **AI Parking Prediction:** Dashboard graph with simulated data: 8 AM (72%), 9 AM (48%), 10 AM (31%), 11 AM (55%), 12 PM (68%), with prominent `[SIMULATED DATA]` demo labeling.
7. ✅ **AI “Find Best Parking”:** Recommendation wizard evaluating walking distance, congestion, and vehicle type: *“Recommended: Zone A, Slot A-12 • 120 m away • Approx. 2 min walk”*.
8. ✅ **Parking Reservation:** Full booking modal generating Reservation ID (`RTC-CSE-2026-9481`), Slot #, Date/Time window, and digital QR Code pass.
9. ✅ **QR Entry / Exit:** Simulated boom-barrier gate terminal with animated lifting arm, camera laser scan line, license plate matching, and check-in/out logging.
10. ✅ **My Vehicles:** Fleet manager to register vehicle number, vehicle type, make & model, color, and default vehicle indicator.
11. ✅ **Parking History:** Searchable table logging date, vehicle number, zone, slot, entry time, exit time, duration, and fee status.
12. ✅ **Notifications:** Real-time alert drawer with examples: *“Zone B is almost full.”*, *“Your parking reservation starts in 15 minutes.”*, *“Zone C has more available spaces.”*, *“High parking demand expected at 9:00 AM.”*
13. ✅ **Report Parking Problem:** Incident desk modal for: Incorrect availability, Blocked slot, Unauthorized parking, Damaged parking area, EV charger issue, and Security issues.
14. ✅ **EV and Accessible Parking:** Dedicated view with live charger output specs (7.4kW / 22kW) and zero-barrier wheelchair ramp access.
15. ✅ **Admin Dashboard:** Total 500, Occupied 312, Available 188, Reserved 42, Today's 1,284; zone charts, peak-hour analytics, and supervisor controls.
16. ✅ **Admin AI Insights:** Prominently labeled simulated insights: *“Zone A may reach full capacity soon.”*, *“Zone E is currently underused.”*, *“Highest demand occurs during morning peak hours.”*, *“Redirect vehicles to Zone C to reduce congestion.”* with an executable reroute button!
17. ✅ **ParkAI Chatbot:** Floating interactive assistant answering queries like: *“Where can I park near the CSE block?”*, *“Which zone has the most spaces?”*, *“Find an EV parking space.”*, *“What is the nearest available parking?”*, and *“When is parking expected to be crowded?”*
18. ✅ **Demo Mode Controller:** Sticky floating evaluator toolbar to live-toggle:
    - 🟢 *Normal Occupancy*
    - ⚡ *High Demand (9:15 AM Peak)*
    - 🛑 *Zone A Full (Triggers AI Reroute)*
    - 🎟️ *Simulate New Booking*

---

## 🧠 5. How AI Functionality is Simulated
To satisfy academic integrity and prototype presentation guidelines, **all AI components are clearly labeled as simulated / demo models**:

1. **Hourly Occupancy Forecasting (Time-Series Simulation):**
   - In production, this would use an **LSTM (Long Short-Term Memory)** recurrent neural network or **XGBoost Regressor** trained on historical gate timestamp logs, weather conditions, academic exam schedules, and holiday calendars.
   - In this prototype, the curve is computed via a mathematical hourly distribution function reflecting campus shift changes (e.g. morning lecture arrivals at 8:45 AM leading to the 10:00 AM 31% free slot trough).

2. **AI Best Parking Recommendation (Multi-Criteria Heuristic Scoring):**
   - Simulated using a weighted euclidean scoring function:
     $$\text{Score} = w_1 \cdot \left(1 - \frac{\text{Distance}}{D_{\max}}\right) + w_2 \cdot \text{AvailabilityRatio} + w_3 \cdot \text{SlotTypeMatch}$$
   - Prioritizes proximity to the user's destination (e.g. Zone A for CSE Block) while filtering for matching amenities (EV charger or wheelchair ramps).

3. **ParkAI Natural Language Assistant:**
   - Simulated with an intent classification pattern matcher that dynamically queries the application's live React state (`slots`, `zones`, `predictions`, `user`), formatting answers with markdown and actionable deep-links.

4. **Dynamic Traffic Rerouting:**
   - Simulates a rule-based expert system that detects when Zone A exceeds 90% capacity and shifts suggested navigation routes to Zone C and Zone D.

---

## 💻 6. How to Run the Project Locally

### Prerequisites
- Node.js (v18 or higher installed on Windows/Mac/Linux)
- npm

### Installation & Launch Steps
1. Open PowerShell or Command Prompt in the project folder:
   ```bash
   cd "c:\Users\user\Desktop\project ai"
   ```
2. (Optional if already installed) Install project dependencies:
   ```bash
   npm.cmd install
   ```
3. Start the local development server:
   ```bash
   npm.cmd run dev
   ```
4. Open your web browser and navigate to:
   ```
   http://localhost:3000
   ```
5. To create a production build:
   ```bash
   npm.cmd run build
   ```

---

## 🔮 7. Real-World Implementation & Upgrade Blueprint

To transition this high-fidelity prototype into an enterprise smart-campus IoT deployment:

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                       Physical Real-World IoT Architecture                  │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                             │
│  [Campus Entry / North & South Gates]                                       │
│    ├── ANPR Cameras (YOLOv8 / OpenCV running on Raspberry Pi 5 / Jetson)    │
│    ├── RFID Windshield Sticker Readers (UHF 865-868 MHz)                    │
│    └── Microcontroller (ESP32) commanding Industrial Boom Barrier Servos    │
│                                                                             │
│  [Individual Parking Slots]                                                 │
│    ├── Option A: Overhead Fisheye 4K Cameras running Mask R-CNN (Slot Occ)  │
│    └── Option B: In-ground Geomagnetic / Ultrasonic Sensors (LoRaWAN / Zig) │
│                                                                             │
│  [Edge & Cloud Backend]                                                     │
│    ├── MQTT Broker (EMQX / Mosquitto) for sub-second slot telemetry         │
│    ├── Python FastAPI / Node.js Backend Server                              │
│    ├── PostgreSQL + PostGIS (Spatial Database for routing & coordinates)     │
│    └── Machine Learning Pipeline: PyTorch LSTM for occupancy forecasting   │
│                                                                             │
│  [Client Applications]                                                      │
│    ├── Progressive Web App (PWA) / React Native Mobile App for Students     │
│    └── Outdoor LED Variable Message Signs (VMS) at Campus Intersections     │
└─────────────────────────────────────────────────────────────────────────────┘
```

1. **Hardware Sensor Layer:**
   - **Overhead Vision AI:** Mount wide-angle 4K IP cameras on light poles over Zone A–E running a YOLOv8 or Mask R-CNN model to monitor 30–50 slots simultaneously without digging into asphalt.
   - **Gate Hardware:** High-speed automatic number plate recognition (ANPR) cameras paired with an ESP32 relay module controlling the boom barrier arm via MQTT.

2. **Communication & Cloud Backend:**
   - **Protocol:** MQTT / WebSockets for low-latency updates whenever a car enters or leaves a slot.
   - **Backend API:** FastAPI (Python) or Express.js with PostgreSQL & Redis caching for instant QR pass verification.

3. **Machine Learning Model Upgrades:**
   - Replace simulated trends with a production **Graph Neural Network (GNN)** or **LSTM** trained on semester timetables, weather forecasts, and historical college attendance patterns.

---

## 🎓 Academic Credit & Attributions
- **Author:** Aakash RB
- **Department:** Computer Science and Engineering (CSE)
- **College:** Rathinam Technical Campus
- **Batch:** 2025–2029
- **Tools Used:** React 18, TypeScript, Tailwind CSS, Lucide React, Canvas Confetti, Vite.
