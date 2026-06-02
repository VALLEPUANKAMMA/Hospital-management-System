# 🏥 Hospital Management System

## 📖 Overview

Hospital Management System is a menu-driven application developed in C Programming to manage patient records, doctor details, appointments, admission status, and hospital data efficiently.

The project uses Singly Linked Lists (SLL), Structures, File Handling, Typedefs, Enums, and Modular Programming concepts to provide a complete hospital record management solution.

---

## 🎯 Objective

The objective of this project is to:

- Maintain patient records efficiently.
- Manage doctor-patient appointments.
- Prevent duplicate patient account creation.
- Store hospital data permanently using files.
- Implement modular and reusable code.
- Provide an easy-to-use menu-driven interface.

---

## ✨ Features

### ✅ Add Patient Account

Register new patient accounts with:

- Account Number
- Patient Name
- Contact Number
- Room Number
- Doctor Name
- Disease Name
- Joining Date
- Discharge Date
- Admission Status

---

### ✅ Book Appointment

Book appointments with doctors for registered patients.

---

### ✅ Print Records

Display patient information using various filters:

1. Print all patient details
2. Print specific patient details
3. Print doctor-wise patient details
4. Print disease-wise patient details

---

### ✅ Search Patient

Search patient records using:

- Account Number
- Patient Name
- Contact Number

---

### ✅ Modify Patient Details

Update:

- Contact Number
- Room Number
- Doctor Name
- Disease Name
- Admission Status
- Discharge Date

---

### ✅ Delete Patient Record

Remove patient records from the hospital database.

---

### ✅ Save Data

Store all patient information permanently using file handling.

---

## 📋 Menu

```text
------------------ MENU ------------------

A : Book appointment to visit doctor

P : Print Function
    1. Print all patients complete details
    2. Print only specific patient details
    3. Print only specific doctor patients details
    4. Print specific issue patients details

S : Save all data to file

F : Find/Search patient

M : Modify patient details

X : Delete patient record

Q : Quit application
```

---

## 🏗️ Data Structure

```c
typedef struct patient
{
    int account_no;
    char patient_name[50];
    char contact_no[15];
    int room_no;

    char doctor_name[50];
    char disease_name[50];

    char joining_date[20];
    char discharge_date[20];

    int admission_status;

    struct patient *next;

}PATIENT;
```

---

## 📂 Project Structure

```text
Hospital_Management_System/
│
├── include/
│   └── hospital.h
│
├── src/
│   ├── main.c
│   ├── create_account.c
│   ├── appointment.c
│   ├── print.c
│   ├── search.c
│   ├── modify.c
│   ├── delete.c
│   ├── save.c
│   └── load.c
│
├── data/
│   └── patients.dat
│
├── Makefile
│
└── README.md
```

---

## ⚙️ Technologies Used

- C Programming
- Structures
- Typedef
- Enum
- Union
- Singly Linked List (SLL)
- Dynamic Memory Allocation
- File Handling
- Makefile
- Linux Programming

---

## 🔒 Validation Rules

### Account Number

- Must be unique.
- Duplicate account numbers are not allowed.

### Patient Name

- Duplicate names are allowed.

### Patient History

- If a patient visits again, new records can be added while preserving previous information.

---

## 💾 File Handling

Patient records are stored using file handling.

Functions used:

```c
save_data();
load_data();
sync_file();
```

Benefits:

- Permanent storage
- Easy retrieval
- Data backup support

---

## 🛠️ Functions Used

### Account Management

```c
create_account();
modify_account();
delete_account();
```

### Appointment Management

```c
book_appointment();
```

### Search Operations

```c
search_patient();
```

### Print Operations

```c
print_all_patients();
print_specific_patient();
print_doctor_patients();
print_disease_patients();
```

### File Operations

```c
save_data();
load_data();
sync_file();
```

---

## 🔨 Build Instructions

Compile the project using:

```bash
make
```

Clean generated files:

```bash
make clean
```

---

## ▶️ Run

Execute the application:

```bash
./hospital
```

---

## 📸 Project Images

### 🔌 Hardware / Development Setup

Add project setup image here:

```
images/setup.png
```

### 🖥️ Application Menu

Add menu screenshot here:

```
images/menu.png
```

### 📋 Patient Record Management

Add patient details screenshot here:

```
images/patient_record.png
```

### 🔍 Search Functionality

Add search operation screenshot here:

```
images/search.png
```

---

## 🚀 Future Enhancements

- Doctor Management Module
- Billing System
- Pharmacy Management
- Medical History Tracking
- Login Authentication
- Admin Dashboard
- ICU Room Allocation
- Emergency Patient Handling
- Report Generation

---

## 📚 Concepts Covered

- Structures
- Typedef
- Enum
- Union
- Linked List
- Dynamic Memory Allocation
- File Handling
- Makefile
- Modular Programming
- Data Validation

---

## 👨‍💻 Author

**AK**

Embedded Systems Engineer

---

## 📜 License

This project is developed for educational and learning purposes.

---
⭐ If you found this project useful, consider giving it a star on GitHub.
