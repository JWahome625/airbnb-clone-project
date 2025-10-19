# airbnb-clone-project
A comprehensive, real-world application designed to simulate the development of a robust booking platform like Airbnb. The application should allow users to make  bookings and will use Django for the backend.

## Team Roles
 Backend Developer- responsible for designing, building and maintaining the booking system 
 Database Administrator- designs, builds and maintains DBs to ensure they are       reliable and secure

 ## Technology Stack
 Django - a web framework for building RESTful APIs
 PostgreSQL - An object oriented relational database.
 GraphQL - a data query manipulation language that is highly declarative. 

## Database Design Overview
Entities in our project:
Users - an owner can have multiple properties
      - a guest can make multiple bookings
      - a guest can make payments for multiple bookings

Properties - belongs to a user who is an owner
           - can have multiple bookings
           - can only be booked to one user at a time

Bookings - made by a guest 
         - is made for a specific property
         - has one payment record

Payments - belongs to a booking
          - made by a guest
          -a booking can have multiple payments

Reviews  - can be written by a guest on the property
          - can be written by a host on the user
          - User/Property can have many reviews

## Feature Breakdown

**User Management 👤**
Allows for the registration, log in and management of user profiles. It limits access of the different user profiles to ensure security. Improves user experience based on the profile by customizing

**Property Management 🏠**
Used to manage the properties in terms of listing, updating availability, editing/deleting the listing etc. Allows for host users to market their listing

**Booking system 📅**
Primarily used to search property, check availability and make reservations. It ensures that properties are not double booked and they are constantly updated. 

**Payment Processing 💳**
Manages payments to accept the different available methods e.g card and to ensure they are secure. Tracks payment status and records the transactions. 

**Review and ratings ⭐**
A guest can give their feedback on their stay and service quality. Hosts can also give feedback on their guests conduct. This promotes good service and good conduct. 


##  API Security Overview

**Authentication 🔐**
Verifies user identity to ensure only the account owners access their accounts. Eliminates and minimizes identity theft that can lead to fraud. 

**Authorization 🧾**
Limits what users can do on the system i.e users can only perform actions that they are allowed to.

**Rate Limiting 🚫**
This limits the number of system requests that can be done in a certain time frame. 

**Data Encryption 🔒**
This protects personal and financial information by concealing it in a way that even when accessed is unreadable.


## CI/CD Pipeline Overview

**CI/CD Pipeline**

Set of practices and tools that automate the building, testing and deployment of software. They are important because they ensure quality, efficiency and quick turn around. 

**Tools used for CI/CD**
Github Actions -for automation and workflow management from Github. 
Docker - For containerization 
Jenkins - for customizable CI/CD pipelines

