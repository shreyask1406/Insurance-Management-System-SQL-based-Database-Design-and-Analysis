# Insurance-Management-System-SQL-based-Database-Design-and-Analysis

## Introduction
Insurance is a critical component in modern life, offering protection and security. As the insurance industry grows, efficient data management becomes essential. This project focuses on creating a database for an "Insurance Company," dealing with health, car, and home insurance policies.

## Database Design
The project aims to develop a database for an insurance company that offers health, car, and home insurance policies. The database encompasses multiple branches, each with agents responsible for customer interactions. The database tables include Company, Agent, Customer, Payment, Policy, Claim, Health, Car, Home, Cust_Policy, and Claim_Policy, all interconnected to efficiently manage insurance-related data.

## Relational Model
The relational model of the insurance management system is designed to effectively organize and manage the data associated with the insurance company's operations. It comprises a set of interconnected tables that store essential information related to branches, agents, customers, policies, payments, claims, and specific insurance types. This model establishes relationships between different entities, enabling seamless retrieval and analysis of data.

The primary tables in the relational model include:
* Company: Captures details about the company's branches, such as Branch_ID, number of employees, city, and zipcode.
* Agent: Stores agent-specific information like Agent_ID, email, name, phone number, and associated Branch_ID.
* Customer: Holds customer data, including Customer_ID, date of birth, name, phone number, email, policy type, address, and Agent_ID.
* Payment: Contains payment-related details like bank account number, billing ID, payment date, amount, and Customer_ID.
* Policy: Stores policy-related information like Policy_no, tenure, start date, end date, premium, coverage, and associated Branch_ID.
* Claim: Stores data related to claims, including Claim_ID, amount issued, claim status, issued date, and related Billing_ID.
* Health: Captures specific health insurance details, such as Health_ID, medical history, associated hospital, treatment insured, and associated Policy_no.
* Car: Contains car insurance-specific information like Car_no, model, registration year, and associated Policy_no.
* Home: Stores home insurance details, including Home_no, type, address, year built, area, and associated Policy_no.
* Cust_Policy: Establishes the relationship between customers and policies, storing Customer_ID and Policy_no.
* Claim_Policy: Represents the relationship between claims and policies, storing Claim_ID and Policy_no.

## MySQL Implementation and Analysis 
### Key Problem Statements:

* Number of customers and agents in each city.
* Top-performing agents based on the number of policies.
* List of customers with multiple policies.
* Annual change in health insurance policies (impact of Covid).
* Year-wise revenue analysis.
* Categorization of insurance policies by premium amount and customer count.
* Age group of customers interested in insurance.

### Connecting Database to Python
MySQL is connected to Python using mysql.connector. Visualizations are created using Python to analyze the problem statements.

## MongoDB Implementation
In addition to the relational model, we've also implemented the insurance management system using MongoDB, a powerful NoSQL database.The MongoDB implementation parallels the relational model in addressing specific problem statements. By leveraging MongoDB Compass, we executed queries to extract meaningful insights from the collections. This included determining the number of customers and agents in a particular city, identifying the top-performing agents based on the number of policies, and obtaining a list of different home types along with their age and area for home insurance. MongoDB's schema flexibility and powerful querying capabilities made it possible to derive valuable information from these scenarios.

## Features and Future Scope
* Triggers for payment validation.
* Automated email notifications for customer birthdays.
* Interactive user interface for data entry.
* Employee records for comprehensive analysis.

## Conclusion
The "Insurance Management System" project offers efficient data management and analysis. The SQL-based database, coupled with Python, facilitates insightful decision-making for insurance companies.

For detailed project components and code, refer to the project repository and documentation.
