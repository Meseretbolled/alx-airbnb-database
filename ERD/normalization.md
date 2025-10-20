# Airbnb Database Normalization (Up to 3NF)

# First Normal Form (1NF)
- Each attribute contains atomic (indivisible) values.
- Each record is unique, identified by a primary key.
All tables (`User`, `Property`, `Booking`, `Payment`, `Review`, `Message`) are in 1NF.

# Second Normal Form (2NF)
- The database is already in 1NF.
- All non-key attributes depend on the entire primary key.

 Each table has a single-column primary key (UUID), so no partial dependency exists.


# Third Normal Form (3NF)
- The database is already in 2NF.
- No transitive dependency (non-key attributes only depend on the primary key).

✅ All tables meet 3NF:
| Table   | Primary Key  | Dependency                       | Status |
|-------- |--------------|--------------------------------- |---------
| User    | user_id      | All fields depend on user_id     | approved|
| Property| property_id  | All fields depend on property_id | approved|
| Booking | booking_id   | All fields depend on booking_id  | approved|
| Payment | payment_id   | All fields depend on payment_id  | approved|
| Review  | review_id    | All fields depend on review_id   | approved|
| Message | message_id   | All fields depend on message_id  | approved|
 
Conclusion: 
The Airbnb database design satisfies **Third Normal Form (3NF)** — ensuring no redundancy and improved data integrity.
