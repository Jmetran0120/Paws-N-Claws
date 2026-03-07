# Paws N Claws - Modernizing Pet Care [cite: 2]
This repository contains the web application for Paws N Claws, designed to modernize service delivery and operational management[cite: 14]. [cite_start]The system features an automated online booking system and centralized customer data management[cite: 142, 144].

#Team: Group Singapore [cite: 6]
CHANG, Dash Michael L. [cite: 7]
CORTES, Juan Diego P. [cite: 7]
METRAN, Josh [cite: 7]
TAN, Marc Joshua [cite: 8]
RAMOS, Nathan Cedric G. [cite: 9]
VILLEGAS, Leila Janine T. [cite: 9]

## Database Schema (Supabase) 
Our database is hosted on Supabase and follows this ERD structure

**CUSTOMER**: Customer_ID (PK), First_Name, Last_Name, Phone_Number, Email 
**EMPLOYEE**: Employee_ID (PK), Employee_Name, Employee_Bio, Employee_Specialization 
**SERVICE**: Service_ID (PK), Service_Name, Service_Description, Service_Price 
**PET**: Pet_ID (PK), Customer_ID (FK), Pet_Name, Pet_Type, Pet_Breed, Pet_Size, Special_Notes 
**APPOINTMENT**: Appointment_ID (PK), Customer_ID (FK), Employee_ID (FK), Pet_ID (FK), Appointment_Date, Start_Time, Total_Price, Status, Special_Notes 
**PAYMENT**: Payment_ID (PK), Appointment_ID (FK), Amount, Payment_Method 

## How to connect to the database
1. Duplicate the `.env.example` file and rename it to `.env.local`.
2. Ask the database administrator for the Supabase URL and Anon Key to paste into your local file.
