

# 🗓️ Appointment Scheduler

A **web application** for managing and scheduling appointments between service providers and customers. Built with **Spring Boot** and **MySQL**, this system allows admins, providers, and customers to handle bookings, notifications, and invoices efficiently.

---

## 🚀 Key Features

* **Role-based access:** Admin, Provider, Customer
* **Appointment management:** Book, cancel, and track appointments
* **Provider scheduling:** Individual working hours, breaks, and availability
* **Notifications:** Automatic email alerts for bookings, cancellations, and rejections
* **Invoice generation:** Create invoices automatically for completed appointments
* **Secure login:** Authentication and role-based access control

---

## ⚙️ Setup Instructions

1. **Clone the repository:**

```bash
git clone https://github.com/yeahmeash/Schedule-manager.git
cd Schedule-manager
```

2. **Create MySQL database:**

```sql
CREATE DATABASE appointments;
```

* Import the schema from `src/main/resources/appointments.sql`.

3. **Configure application properties:**

Edit `src/main/resources/application.properties` to set:

* Database URL, username, and password
* Mail server credentials
* JWT secret for authentication

4. **Run the application:**

```bash
mvn spring-boot:run
```

* Access the app at `http://localhost:8080`.

---

## 👥 User Roles

* **Admin:** Manage providers, services, and all appointments. Can generate invoices and view system reports.
* **Provider:** Define working hours, breaks, and services offered. View only their own appointments.
* **Customer:** Book appointments, view schedule, and manage cancellations.

---

## 📌 Booking Workflow

1. Customer selects a service.
2. Customer chooses a provider and available date/time.
3. Booking is confirmed and recorded in the system.
4. Notifications are sent via email for creation, cancellation, or rejections.
5. System tracks appointment status: Scheduled → Completed → Confirmed → Invoiced.

---

## 🛠️ Technologies Used

* **Backend:** Spring Boot, Java, MySQL
* **Frontend:** HTML, CSS, JavaScript, Thymeleaf
* **Other Tools:** FullCalendar for scheduling, PDF generation for invoices, JWT for authentication

---

## 📄 License

This project is licensed under the **MIT License**.


