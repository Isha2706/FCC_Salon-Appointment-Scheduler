# 💇‍♀️ Salon Appointment Scheduler

A terminal-based **Bash + PostgreSQL** application that allows users to schedule appointments for a salon. This project is part of the **FreeCodeCamp Relational Database Certification**.

## 📖 Project Overview

The Salon Appointment Scheduler lets users:

- View a list of available salon services
- Enter their phone number to retrieve or register their name
- Book an appointment for a selected service
- Store all appointment and customer data in a PostgreSQL database

## 🛠 Technologies Used

- **Bash** – scripting the logic and user interaction
- **PostgreSQL** – managing the database for services, customers, and appointments

## 📂 Files Included

- `salon.sh` – The Bash script that runs the interactive scheduler
- `salon.sql` – SQL script to create and set up the database schema

## 🗃️ Database Schema

The project uses a PostgreSQL database named `salon`, which includes:

- `services` – List of available salon services (e.g., haircut, manicure)
- `customers` – Stores customer phone numbers and names
- `appointments` – Stores appointment time, service, and customer

## ▶️ How to Run

### 1. Set Up the Database

```bash
psql -U postgres -f salon.sql
```

### 2. Make the Bash Script Executable
```bash
chmod +x salon.sh
```

### 3. Run the Scheduler
```bash
./salon.sh
```

Follow the prompts to select a service, enter your phone number and name, and book your appointment.

## 💡 Features

- User-friendly command-line interface
- Dynamic service listing from the database
- Reuse of customer data via phone number lookup
- Error handling for invalid inputs
- Clean and modular SQL design

## 📜 Certification

This project is part of the [FreeCodeCamp.org](https://www.freecodecamp.org/) **Relational Database Certification**.
