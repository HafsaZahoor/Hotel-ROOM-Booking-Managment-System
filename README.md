# 🏨 Hotel Room Booking System (SQL Project)

This project is a full-featured hotel room booking system built entirely with SQL. It covers everything from database schema design, room and guest management, availability tracking, booking logic, and detailed reporting using SQL queries and views.

---

## 📌 Project Objective

The main goal of this project is to design and implement a **hotel booking database system** that can:
- Handle guest and room details
- Manage different room types and capacities
- Process bookings with status tracking (Pending, Confirmed, Cancelled, Completed)
- Ensure availability and prevent booking overlaps
- Generate business reports like room utilization, guest summaries, and revenue

---

## 🛠️ Technologies Used

- **MySQL** – Used for database creation, querying, and view generation
- **SQL DDL & DML** – Used for schema design, data insertion, logic, and reporting

---

## 🧱 Database Structure

### Tables Created:
- `Guests` – Stores guest info (name, email, phone)
- `RoomTypes` – Types of rooms (Single, Double, Suite) with capacity and pricing
- `Rooms` – Physical room units linked to a type
- `Bookings` – Stores booking records with check-in/out, guest, and room reference

### Additional:
- **Indexes** on key columns (e.g., room type, booking status)
- **CHECK constraint** to ensure `check_in < check_out`
- **ENUM** type for `booking_status`

---

## 🔍 Key Functional Features

### ✅ Core Booking Logic:
- Insert and update bookings
- Prevent double-booking via availability checks
- Auto-confirm bookings if conditions are met

### 📊 Reporting and Views:
- `AvailableRooms` – Shows rooms not booked for the next 30 days
- `GuestBookingSummary` – Aggregates total nights and bookings per guest
- `RoomStatus` – Displays if a room is **Occupied** or **Available** today
- Daily booking counts and guest overlaps by date
- Room utilization (% occupancy calculation)
- Revenue calculation per room type

### 📌 Additional Features:
- Fetch today's check-ins
- Filter bookings by guest or room
- Cancel or find overlapping bookings

---

## 📂 Sample Data Included

- **Guests**: 3 sample records
- **Room Types**: Single, Double, Suite
- **Rooms**: Room numbers (101, 102, 201) mapped to types
- **Bookings**: Various scenarios (Confirmed, Cancelled, Pending, Overlapping)

---

## 🚀 How to Use

1. Copy and run the SQL file in any **MySQL-compatible** database system.
2. Start with `DROP DATABASE IF EXISTS` and `CREATE DATABASE HotelBookingDB;`
3. Execute the full script to set up schema, insert sample data, and create views.
4. Use the **queries at the end** to test reports, availability, and booking logic.

---

## 📌 Example Use Cases

- 🔹 View all rooms that are available for booking in the next 30 days  
- 🔹 Track guest activity and total nights booked  
- 🔹 Identify room types with highest usage or revenue  
- 🔹 Confirm a pending booking only if there’s no overlap  
- 🔹 Show today’s check-ins and guest summaries

---

## 📧 Contact

**Hafsa Zahoor**  
📬 [hafsazahoor63@gmail.com](mailto:hafsazahoor63@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/hafsa-zahoor-6a4b01373?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app)

---

## 🏷️ Tags

`#SQL` `#HotelBookingSystem` `#MySQLProject` `#DatabaseDesign` `#BookingSystem` `#RoomAvailability` `#DataModeling` `#SQLViews`

