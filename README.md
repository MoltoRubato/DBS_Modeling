# DBS_Modeling

## Overview
This project is a MySQL-based relational database design for an electric vehicle (EV) charging station system. The system manages information about charging stations, electric vehicles, charging events, and associated facilities such as cafés or restaurants. The database supports querying for various business requirements like tracking charging station ownership, electric vehicle usage, and facility-related discount coupons.

## Key Features
- **Charging Stations**: Stores information about charging stations, including address, operating hours, and associated outlets. Each outlet has unique charging rates and costs for peak and off-peak hours.
- **Electric Vehicles**: Tracks EVs by VIN, manufacturer, model, battery capacity, and the company that manufactures them.
- **Charging Events**: Records each charging event, including which outlet was used, start and end times, and any discount coupons applied.
- **Facilities**: Manages facilities (like cafés or restaurants) that may be associated with charging stations, including discount coupons for charging events.
- **Companies**: Tracks companies manufacturing EVs, their CEOs, and their involvement in owning charging stations.

## Models
- **Conceptual Model**: Designed using Chen's notation, representing the business entities and their relationships.
- **Physical Model**: Implemented in MySQL Workbench using Crow’s Foot notation, providing the detailed database schema.

## Business Requirements
The database supports various queries including:
- Ownership tracking for companies like Tesla.
- Finding charging stations with specific facilities (e.g., cafés).
- Calculating total income from charging outlets.
- Managing charging event details and associated discounts.

## Setup
1. Clone the repository.
2. Import the provided `.mwb` file into MySQL Workbench.
3. Execute the schema and queries as described.

## Assumptions
- Opening and closing hours for stations and facilities are the same every day.
- A single discount coupon can be applied to a charging event.
- Assumptions regarding entity relationships are detailed in the attached PDF.

## Tools Used
- **MySQL Workbench** for database modeling.

## Contributors
- Ryan Huang
- INFO20003 Teaching Team (Question Provider)
