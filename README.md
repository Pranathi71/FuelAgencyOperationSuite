


# 🚀 **FuelPro - Fuel Agency Operation Suite**

**FuelPro** is a web-based system designed for managing **customers**, **suppliers**, **cylinders**, and generating **reports** for a fuel agency.

It allows:
- Admins to manage customer and supplier data, track cylinder inventories, and generate reports.
- Customers to easily book cylinders and view their booking history.

---

## 🔧 **Features**

### 🛠️ **Admin Features**
- **Customer Management**: Add, edit, and delete customer profiles.
- **Supplier Management**: Add, edit, and manage supplier details.
- **Cylinder Management**: Track and manage available cylinders, assign to customers, and update inventory.
- **Booking Management**: View and manage all customer bookings.
- **Reports**: Generate reports for customer bookings, inventory status, and supplier details.
- **Email**: Automatic email is triggered for every action.

### 👥 **Customer Features**
- **Cylinder Booking**: Customers can book cylinders through the system.
- **View Booking**: View status of bookings, delivery details, and booking history.
- **Email**: Booking details are sent via email for confirmation.

---

## 🧪 **Steps to Run FuelPro**

### ✅ **Step 1: Install Necessary Packages**

Run the following command in both **Frontend** and **Backend** project directories:

```bash
mvn clean install
```

📌 **Note**:  
- Make sure no previous data/tables exist in the `FuelAgency` database.  
- Update the `application.properties` file with the correct database credentials.

---

### 🚀 **Step 2: Run the Project**

Run this command to start both frontend and backend:

```bash
mvn clean spring-boot:run
```

💡 Ensure **MySQL** and **Apache** are running if you’re using **XAMPP**.

---

### 🧪 **Step 3: Create Dummy Data Using POSTMAN**

Use **POSTMAN** to send dummy data to your backend.

#### Endpoint:

```http
POST http://localhost:8080/api/users
```

#### JSON Body:

```json
{
  "firstName": "Pranathi",
  "lastName": "Tatavarthi",
  "email": "XXXX.com",
  "phone": "4394568692",
  "address": "234 Main Street, Malborne",
  "connectionType": "DOMESTIC",
  "connectionStatus": "ACTIVE",
  "role": "ADMIN"
}
```

---

## 🌐 **Accessing the Application**

- Open: [http://localhost:1000/](http://localhost:1000/)
- Login as **Admin** using the credentials (User ID and Password) received via email.

---

## ⚙️ **Workflow Summary**

1. Create a **Customer** from Customer Management.
2. Add a **Supplier** from Supplier Management.
3. Add a **Cylinder** from Cylinder Management.
4. Login as **Customer** using credentials sent via email.

---

✨ Enjoy managing your fuel agency with **FuelPro**!

