# [cite_start]Paws N Claws - Modernizing Pet Care [cite: 2]

[cite_start]This repository contains the web application for Paws N Claws, designed to modernize service delivery and operational management[cite: 14]. [cite_start]The system features an automated online booking system and centralized customer data management[cite: 142, 144].

## [cite_start]Team: Group Singapore [cite: 6]
* [cite_start]CHANG, Dash Michael L. [cite: 7]
* [cite_start]CORTES, Juan Diego P. [cite: 7]
* [cite_start]METRAN, Josh [cite: 7]
* [cite_start]TAN, Marc Joshua [cite: 8]
* [cite_start]RAMOS, Nathan Cedric G. [cite: 9]
* [cite_start]VILLEGAS, Leila Janine T. [cite: 9]

## [cite_start]Database Schema (Supabase) [cite: 99]
[cite_start]Our database is hosted on Supabase and follows this ERD structure[cite: 99]:

* [cite_start]**CUSTOMER**: Customer_ID (PK), First_Name, Last_Name, Phone_Number, Email [cite: 100, 101, 102, 103, 104, 105]
* [cite_start]**EMPLOYEE**: Employee_ID (PK), Employee_Name, Employee_Bio, Employee_Specialization [cite: 122, 123, 124, 125, 126]
* [cite_start]**SERVICE**: Service_ID (PK), Service_Name, Service_Description, Service_Price [cite: 135, 136, 137, 138, 139]
* [cite_start]**PET**: Pet_ID (PK), Customer_ID (FK), Pet_Name, Pet_Type, Pet_Breed, Pet_Size, Special_Notes [cite: 127, 128, 129, 130, 131, 132, 133, 134]
* [cite_start]**APPOINTMENT**: Appointment_ID (PK), Customer_ID (FK), Employee_ID (FK), Pet_ID (FK), Appointment_Date, Start_Time, Total_Price, Status, Special_Notes [cite: 112, 113, 114, 115, 116, 117, 118, 119, 120, 121]
* [cite_start]**PAYMENT**: Payment_ID (PK), Appointment_ID (FK), Amount, Payment_Method [cite: 106, 107, 108, 109, 110]

## How to connect to the database
1. Duplicate the `.env.example` file and rename it to `.env.local`.
2. Ask the database administrator for the Supabase URL and Anon Key to paste into your local file.
