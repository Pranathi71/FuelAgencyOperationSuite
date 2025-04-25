FuelPro - Fuel Agency Operation Suite
FuelPro is a web-based system designed for managing customers, suppliers, cylinders, and generating reports for a fuel agency. It allows admins to manage customer and supplier data, track cylinder inventories, and generate reports. Customers can easily book cylinders and view their booking history.

Features
Admin Features:
Customer Management: Add, edit, and delete customer profiles.

Supplier Management: Add, edit, and manage supplier details.

Cylinder Management: Track and manage available cylinders, assign to customers, and update inventory.

Booking Management: Admins can view and manage all customer bookings.

Reports: Generate reports for customer bookings, inventory status, and supplier details.

Email : Automatic email is triggered for every action.

Customer Features:
Cylinder Booking: Customers can book cylinders through the system.

View Booking: Customers can view the status of their bookings , delivery details and track their previous bookings.

Email : booking details are sent to mail for confirmation purpose.

# these are the steps to run FuelPro

**step 1 :**
Install necesaary packages in both Frontend and Backend. Run this

```
mvn clean install
```

command in project directory. make sure there should be no previous data or table in FuelAgency database which you create in your mysql database. If you set the password for your database once check `application.properties` file in Backend project.

**step 2 :**
for running the Frontend and backend project from terminal use this command

```
mvn clean spring-boot:run
```

Remember to start mysql and apache if you are using XAMPP.

**step 3 :**
create dummy data using POSTMAN in customer and cylinder table. Hit these API endpoints as mention below.

### POST http://localhost:8080/api/users

JSON

```
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

### go to http://localhost:1000/ and login as admin with userId and password which where sent on email

### and can be viewed in postman after creating admin with json to first create customer from customer management,

### and then create supplier from supplier management and then add cylinder from cylinder management and

### then login as a customer with customerId and Password which sent on email.
