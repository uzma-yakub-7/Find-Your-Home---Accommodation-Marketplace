# **Software Requirement Specification (SRS)**

## **Project Title:** Find Your Home – Accommodation Marketplace for Tenants

## **1. Introduction**

### **1.1 Purpose**

The purpose of this document is to define the software requirements for Find Your Home, a rental accommodation platform designed to help people easily find rental homes in major cities of Bangladesh, starting with Sylhet and Dhaka. This SRS describes the system’s functionality, scope, constraints, and overall workflow to guide development and evaluation.

### **1.2 Problem Statement**

People moving to cities like Sylhet and Dhaka struggle to find trusted rental housing options. Key issues include:

* Difficulty finding available rentals
* Lack of verified information
* Dependency on brokers
* Time‑intensive physical searching

Existing solutions lack localization for Bangladesh. 
### **1.3 Proposed Solution**

**Find Your Home** is an online rental marketplace connecting:

* **Renters/Tenants**
* **House Owners/Landlords**

The system enables property searching, detailed viewing, authentication, booking, and interaction. 

## **2. Scope of the Project**

### **2.1 Initial Scope**

* Target service areas:

  * **Sylhet City**
  * **Dhaka City**
* Accommodation types:

  * Apartments
  * Rooms
  * Houses
  * Shared accommodation

### **2.2 Future Scope**

* Nationwide expansion
* Mobile app (React Native / Flutter)
* AI recommendations and smart filters
* Integrated payment system

## **3. System Overview**

Find Your Home is a web marketplace with roles:

1. **Tenant**
2. **House Owner**
3. **Admin**

The app allows authenticated users to create accounts, list properties, search with filters, and manage bookings. 

## **4. Functional Requirements**

### **4.1 Tenant Features**

* Register and login (email/password)
* Profile management
* Search rental listings

  * By city, area, price range, property type
* Advanced filters (rooms, amenities)
* View listing details

  * Photos
  * Price
  * Facilities
  * Host details
* Booking system

  * Select dates
  * Check availability
* Favorites / Wishlist
* Booking history

### **4.2 House Owner Features**

* Owner registration & login
* Create and manage property listings

  * Title, description
  * Multiple images
  * Price and rent terms
  * Availability calendar
* Update/edit/delete listings
* View booking requests
* Confirm/decline bookings

### **4.3 Admin Features**

* Admin authentication
* Approve/verify listings
* User management

  * Suspend or remove suspicious accounts
* Remove fake or duplicate listings
* Monitor site activity and analytics

## **5. Non‑Functional Requirements**

* **User‑Friendly UI** — intuitive front end
* **Secure Authentication**

  * JWT or session‑based
  * Password hashing
  * Optional OAuth (Google)
* **Fast Search Performance**
* **Responsive Design**
* **Data Protection**
* **Scalability** — support many users & listings
* **Cross‑Browser Compatibility**

## **6. Technologies Used**

### **6.1 Frontend**

* React.js / Next.js
* Tailwind CSS / UI library
* React Router
* Axios for API calls

### **6.2 Backend**

* Node.js
* Express.js
* REST API

### **6.3 Database**

* MongoDB (NoSQL)

### **6.4 Authentication**

* JWT / OAuth (optional Google Auth)


## **7. Dataset Description**

Dataset consists of:

* Property listings

  * Location
  * Price
  * Rooms
  * Amenities
  * Images
* User data

  * Profile
  * Login info (not NID/passport data)
* Booking data

  * Dates
  * Tenant ID
  * Property ID

Data can be *seeded manually for development / demo purposes*.

## **8. System Workflow**

1. User registers or logs in.
2. Tenant searches property listings.
3. Tenant filters and selects a property.
4. Tenant views property detail page.
5. Tenant requests a booking (date selection).
6. Owner reviews and confirms booking.
7. Booking details are stored.
8. Tenant visits property physically and completes verification.

## **9. Application Architecture**

* **Frontend:** React or Next.js with modern UI components
* **Backend:** REST APIs with Express
* **Database:** MongoDB
* **Authentication:** JWT sessions

## **10. Limitations**

* No integrated online payments initially
* No digital storage of NID/passport
* Limited initial service area

## **11. Conclusion**

Find Your Home is a web application to modernize the rental search process in Bangladesh, with core features inspired by full‑stack Airbnb clone tutorials. It delivers authenticated user workflows for tenants and owners, scalable design, and usable interfaces for property browsing and bookings — preparing it for future enhancements like mobile apps and smart recommendations.

## **12. Reference **

YouTube Playlist: https://www.youtube.com/playlist?list=PLnE5DGXxG1AqX7BdIt_3_9RVXdDiMTAGl
GitHub Source Code: https://github.com/PardeepBhasin/airbnb-clone

