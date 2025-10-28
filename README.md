# 🎫 Ticket Manager

**Ticket Manager** is a console-based application built with **pure Python**, designed to simulate a real-world customer service ticketing system.  
It allows users to **generate, manage, and analyze tickets** handled by different service desks.  
The system also includes multiple reports and performance analytics, such as identifying the **most active desk**, the **most frequent ticket type**, and the **average waiting time**.

---

## 📌 Features

- **Ticket Generation**
  - Create new tickets by service type (e.g., Repair or Delivery)  
  - Sequential numbering system for each ticket type  
  - Operating hours validation (open between 8:00 and 23:00)

- **Service Desk Management**
  - Assign tickets to desks 1–4  
  - Restrictions by service type (e.g., deliveries only at desk 4)  
  - Records details such as equipment, condition, and observations  

- **Reports & Analytics**
  - General ticket summary  
  - Ticket report by date  
  - Average waiting time per day  
  - Service desk performance report  
  - Revenue report by date  
  - Identification of the busiest desk and most requested ticket type  

- **Additional Functionalities**
  - Calculates waiting time between ticket creation and service  
  - Input validation for text and numerical fields  
  - Persistent storage using custom text-based data handling (`db.py`)  

---

## 🧩 Project Structure
```
ticket-manager/
├── main.py # Main program (menu and control flow)
├── db.py # Data storage, read/write functions
├── manager.py # Analytics and report generation
├── test.txt # Example data file
├── .gitignore
└── README.md
```
---

## 🛠️ Technologies Used

| Technology | Description |
|-------------|-------------|
| **Python 3.x** | Core programming language |
| **datetime** | For time tracking and waiting time calculations |
| **os** | Console interface and screen clearing |
| **Custom Modules (db, manager)** | Data persistence and analytics |

---

## 🚀 How to Run

1. **Prerequisites**
   - Install **Python 3.8 or higher**

2. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/ticket-manager.git
   cd ticket-manager

    Run the application

    python main.py

🧠 Example Workflow

---------- Ticket System ----------

1. Generate Ticket
2. Serve Customer
3. Manage Tickets
4. Exit

Select an option: 1
Service Type:
1. Repair
2. Delivery
> 1

Ticket for Repair created!
Ticket Number: 7

📊 Example of Report Output

=== Service Desk Report (2025-10-28) ===
Desk 1: 35 tickets handled
Desk 2: 28 tickets handled
Desk 3: 40 tickets handled
Desk 4: 22 tickets handled
Most active desk: Desk 3
Most requested ticket type: Repair
Average waiting time: 4m 12s
Total revenue: R$ 2,450.00

🧭 Project Purpose

The main goal of Ticket Manager is to demonstrate logical structuring, data manipulation, and reporting in Python without relying on external frameworks.
It’s designed as both a learning project and a practical simulation of real-world customer service systems.
