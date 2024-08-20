# Project2_SQL_TopDown- Health Insurance Management System

## Overview
This project demonstrates the design and implementation of a relational database for a health insurance management system. The database structure is created using a top-down approach, focusing on key aspects of the system such as customer management, policy administration, claims processing, healthcare provider information, and financial transactions. The project involves creating several interconnected tables, establishing relationships between them, and defining user roles with specific permissions.

## Approach
This project utilizes a top-down approach to database design. We started by identifying the major entities and processes in a health insurance system, then broke these down into more specific components and relationships. This approach allowed us to create a comprehensive and cohesive database structure that effectively models the complexities of health insurance management.

## Project Structure

The project is structured around the following main entities:

1. **Customers**: Stores customer information, including CustomerID, FirstName, LastName, DOB, PhoneNumber, and Email.
2. **Policies**: Contains details about insurance policies such as PolicyID, CustomerID, PolicyType, StartDate, EndDate, and PremiumAmount.
3. **Claims**: Tracks claim information, including ClaimID, PolicyID, ClaimDate, ClaimAmount, and ClaimStatus.
4. **Hospitals**: Manages hospital information with fields like HospitalID, HospitalName, Address, and PhoneNumber.
5. **Doctors**: Stores doctor details including DoctorID, DoctorName, Specialty, PhoneNumber, and HospitalID.
6. **Hospitalizations**: Keeps track of patient hospitalizations, including HospitalizationID, CustomerID, HospitalID, AdmissionDate, DischargeDate, and TotalCost.
7. **Treatments**: Records treatment information such as TreatmentID, HospitalizationID, DoctorID, TreatmentDescription, and TreatmentCost.
8. **Payments**: Manages payment records with fields like PaymentID, CustomerID, PaymentDate, PaymentAmount, and PaymentMethod.

## Database Schema

The database schema includes the following tables:

- Customers
- Policies
- Claims
- Hospitals
- Doctors
- Hospitalizations
- Treatments
- Payments

Each table is designed with appropriate fields and data types to ensure efficient data storage and retrieval.

## Relationships

The database schema includes the following key relationships:

1. Customers to Policies: One-to-Many
2. Policies to Claims: One-to-Many
3. Customers to Hospitalizations: One-to-Many
4. Hospitals to Hospitalizations: One-to-Many
5. Hospitals to Doctors: One-to-Many
6. Hospitalizations to Treatments: One-to-Many
7. Doctors to Treatments: One-to-Many
8. Customers to Payments: One-to-Many

## Roles and Permissions

The system includes various user roles with different levels of access:

1. Administrator: Full access to all tables and data
2. Insurance Agent: Manage customer and policy information, create claims
3. Claims Processor: Process and update claims
4. Healthcare Provider: Manage hospitalizations and treatments
5. Finance Officer: Handle payments and financial records
6. Customer Service Representative: Access customer information and basic policy details
7. Auditor: Read-only access to all tables for audit purposes
8. Customer: Access to their own records (if implementing a customer portal)

Each role has specific permissions designed to ensure data security and maintain the principle of least privilege.

## Contributors

Diksha Jain - 045018
Mohit Vaidya - 045032
Shantanu Bharvirkar - 045052
