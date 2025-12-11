# 🚗 Parking Garage Management System  
*A Software Engineering Project by Muhammed Uwais Adam*

## 📌 Overview  
This project presents a full **software engineering analysis and design** for Eduvos’ proposed Parking Garage Management System. The system aims to:

- Track and manage parking occupancy  
- Reduce congestion inside the garage  
- Allow clients to **find, reserve, and pay** for parking efficiently  
- Automate entry/exit using licence plate recognition  
- Handle real-time spot detection using sensors  

This repository contains the complete set of UML diagrams, scenarios, use-case analysis, class diagram, activity workflows, communication diagram, and state-machine modelling required for a real-world software solution.

---

## 🎯 Problem Summary  
Eduvos identified several issues in its parking facility:

- Inefficient use of parking space  
- Congestion inside the garage as drivers search for open spots  
- No reservation or automated payment system  

The proposed solution introduces:

- Online reservations (daily & monthly)  
- Automated licence plate scanning at entry/exit  
- Sensor-based detection of available parking spots  
- Automatic fee calculation for overstays  
- Email notifications and receipts  

---

## 🧩 Actors in the System  
- **Client**  
- **Eduvos Website / System**  
- **Licence Plate Readers (Entry & Exit)**  
- **Sensors**  
- **Payment Processor**

---

## 🚦 Key Use Cases  
- Reserve a parking space  
- Find available parking spots  
- Pay for parking  
- Update an existing reservation  
- Pay for exceeded parking time  
- Receive parking notifications  

---

## 📝 Scenario Highlights

### **1. Making a Reservation**
- Client enters personal, vehicle, and payment details  
- System validates and stores the data  
- Confirmation email is sent  
- If details are invalid → user must resubmit  

### **2. Updating Reservation (24 hours before)**
- Updates allowed up to 24 hours before reserved date  
- System sends an updated confirmation email  
- If update request is too late → reservation is terminated  

### **3. Arrival at Garage**
- Licence Plate Reader verifies the vehicle  
- Sensors determine open spots  
- If plate differs → system creates a temporary number  

### **4. Payment**
- Registered users pay online  
- Unregistered users pay at a debit machine  
- Overtime fees are calculated automatically  

---

## 🖼️ UML Diagrams Included

### ✔ Use Case Diagram  
Shows interactions between all system actors and the core parking functions.

### ✔ Activity Diagram (with Swimlanes)  
Depicts the flow from reservation to exit, including validations, notifications, and payments.

### ✔ Class Diagram  
Defines main system components:

- ParkingGarage  
- System  
- User  
- Reservation (Daily & Monthly subclasses)  
- Vehicle / BorrowedVehicle  
- Payment  
- Database  
- Sensors, Cameras, Debit Machine  

Relationships include aggregation, association, inheritance, and composition.

### ✔ Communication Diagram  
Shows how the System retrieves booking details, creates Booking objects, and passes formatted lists to the GUI.

### ✔ State Machine Diagram (Account Object)  
Models account states such as:

- Created  
- Registered / Unregistered  
- Reservation Pending  
- Reservation Confirmed  
- Booking Pending  
- Update Booking  
- Cancelled  

---

## 🧪 Recommended Development Methodology  
**Rapid Application Development (RAD)** was chosen because it offers:

- User-centric iteration  
- Fast prototyping  
- Timeboxing  
- High adaptability to changing requirements  

Each RAD cycle improves functionality through user feedback, making it ideal for a system heavily reliant on client interaction and validation workflows.

---

## 📂 Suggested Repository Structure

