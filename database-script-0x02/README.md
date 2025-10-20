# Airbnb Database Seed Script
This script populates the Airbnb database with sample data for testing and development.  
It adds users, properties, bookings, payments, reviews, and messages that simulate real-world scenarios.

# Data Overview
- Users: 4 sample users (2 hosts, 2 guests)
- Properties: 2 sample properties hosted by Alice and Diana
- Bookings: 2 sample bookings made by guests
- Payments: 1 confirmed payment
- Reviews: 2 property reviews
- Messages: 2 example messages between users

# Usage
1. Make sure the database schema (`schema.sql`) has been created.
2. Run the seed script:
   `bash

   "psql -U username -d database_name -f seed.sql"
