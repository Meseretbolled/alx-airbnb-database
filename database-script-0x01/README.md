# Airbnb Database Schema

# Description
This project defines the database schema for an Airbnb-like system that manages:
- Users (hosts and guests)
- Properties listed by hosts
- Bookings made by guests
- Payments for bookings
- Reviews for properties
- Messages between users

# Tables
1. **User** – stores user information.
2. **Property** – represents property listings by hosts.
3. **Booking** – tracks reservations between users and hosts.
4. **Payment** – manages transactions for bookings.
5. **Review** – stores guest reviews and ratings.
6. **Message** – records private messages between users.

# Relationships
- A User (host) can own many Properties.
- A Property can have many Bookings and Reviews.
- A Booking can have one Payment.
- A User can send and receive many Messages.

# Setup
1. Run PostgreSQL or MySQL server.
2. Execute `schema.sql` in your database:
   ```bash
   psql -U username -d database_name -f schema.sql
