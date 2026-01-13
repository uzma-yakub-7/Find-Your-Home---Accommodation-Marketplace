# Software Requirements Specifications (SRS)
# Find Your Home – Accommodation Marketplace

![Project Status](https://img.shields.io/badge/status-Planning-yellow)
![React](https://img.shields.io/badge/React-17.0.2-blue)
![Node.js](https://img.shields.io/badge/Node.js-18.16.0-green)
![Express.js](https://img.shields.io/badge/Express.js-4.18.2-lightgrey)
![MongoDB](https://img.shields.io/badge/MongoDB-6.0.7-brightgreen)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)


## 1. Introduction

### 1.1 Purpose
The purpose of this document is to define the software requirements for **Find Your Home**, a rental accommodation platform designed to help people easily find rental homes in major cities of Bangladesh, starting with Sylhet and Dhaka.  

This SRS describes the system’s functionality, scope, constraints, and overall workflow to guide development and evaluation.

### 1.2 Problem Statement
In cities like Sylhet, many people come from villages or other districts for education, jobs, or medical purposes. Most of them face difficulties such as:

- Not knowing where to find rental houses
- Lack of trusted information
- Dependence on brokers
- Time-consuming physical searching

Unlike foreign countries where platforms like Airbnb are widely used, Bangladesh lacks a localized rental platform suitable for local users.

### 1.3 Proposed Solution
**Find Your Home** is a software platform that connects:

- **House owners** who want to rent their properties  
- **Tenants** who are looking for accommodation

The system provides verified listings, location-based search, and clear rental information to simplify the renting process.


## 2. Scope of the Project

### 2.1 Initial Scope
- Service available in:
  - **Sylhet City**
  - **Dhaka City**
- Rental types:
  - Apartments
  - Rooms
  - Family houses
  - Shared accommodations

### 2.2 Future Scope
- Expansion to **all major cities in Bangladesh**  
- Mobile application version  
- AI-based recommendation system  
- Price prediction and demand analysis

## 3. System Overview
**Find Your Home** works as an online rental marketplace similar to Airbnb but customized for Bangladesh.  

**Users:**
1. Tenants  
2. House Owners  
3. Admin

## 4. Functional Requirements

### 4.1 Tenant Features
- User registration and login  
- Search houses by:
  - City
  - Area
  - Rent range
  - Number of rooms  
- View house details:
  - Images
  - Rent
  - Location
  - Facilities  
- Request booking / contact owner  
- View rental rules and requirements  

> **Important:** Tenants must show valid NID or Passport physically at the time of house entry. The system does not store NID or passport data.

### 4.2 House Owner Features
- Register and login  
- Post house listings  
- Upload house details and photos  
- Set rent and availability  
- Accept or reject tenant requests

### 4.3 Admin Features
- Verify house listings  
- Manage users  
- Remove fake or duplicate listings  
- Monitor system activity

## 5. Non-Functional Requirements
- User-friendly interface  
- Secure authentication system  
- Fast search performance  
- Responsive design (mobile & desktop)  
- Data privacy protection

## 6. Technologies Used

### 6.1 Frontend
- HTML  
- CSS  
- JavaScript  
- React.js (optional)

### 6.2 Backend
- Node.js  
- Express.js

### 6.3 Database
- MongoDB

### 6.4 AI / Machine Learning (Optional / Future)
- Recommendation System based on user preferences  
- Algorithms:
  - KNN (for similarity-based suggestions)
  - Linear Regression (rent trend analysis)

## 7. Dataset Description

**Dataset Type:**
- Rental house data including:
  - Location
  - Rent
  - Number of rooms
  - Facilities

**Dataset Source:**
- Manually collected data  
- Sample datasets from platforms like **Kaggle**  
- Real listings (for demo purposes)


## 8. System Workflow
1. User registers on the platform  
2. Tenant searches for a house  
3. Tenant views details and sends request  
4. House owner reviews the request  
5. Booking is confirmed  
6. Tenant physically visits the house  
7. Tenant provides NID/Passport for offline verification  
8. Final agreement is completed


## 9. Application Type
- Web Application  
- Stack: **MERN** (MongoDB, Express, React, Node)  
- Can be extended to mobile apps in future


## 10. Limitations
- No online payment system (initial phase)  
- No digital storage of NID/passport  
- Limited to two cities initially


## 11. Revenue Model

The website owner earns revenue by monetizing the marketplace platform connecting **house owners** and **tenants**.

### 11.1 Commission on Bookings
- Deduct a percentage of rent for every booking.

| Rent (BDT/month) | Commission % | Platform Earnings (BDT) |
|-----------------|--------------|-------------------------|
| 10,000          | 5%           | 500                     |
| 15,000          | 5%           | 750                     |

- **Workflow:**  
  1. Tenant books a property through the platform  
  2. Platform deducts commission automatically  
  3. Remaining rent is sent to house owner  
  4. Commission goes to website owner

### 11.2 Featured Listings / Premium Placement
- House owners pay extra to highlight listings or appear at the top of search results  
- Example: BDT 200–500 per listing per month

### 11.3 Subscription Model (Optional / Future)
- House owners or tenants can subscribe to premium services:
  - House Owner: unlimited listings, analytics dashboard  
  - Tenant: AI recommendations, early booking alerts

### 11.4 Advertisements
- Local businesses (furniture, movers, cleaners) can advertise on the platform  
- Example: BDT 500–1,000 per ad per month

### 11.5 Optional Add-ons
- Booking protection / security deposit handling  
- Cancellation fees  
- Premium support services

### 11.6 Revenue Flow
1. Tenant books a property → payment goes through platform → commission deducted → balance sent to house owner  
2. House owners pay extra for featured listings → revenue collected directly  
3. Subscriptions and ads provide additional income  
4. Payments are processed via trusted gateways (bKash, Nagad, Rocket, SSLCommerz, Stripe)

**Expected Revenue Example:**  
- 1,000 listings in a city × 5% commission × average rent BDT 10,000 = BDT 500,000/month  
- Expansion to 10 cities → potential monthly revenue = BDT 5,000,000  
- Additional revenue from featured listings & ads = BDT 200,000–500,000/month

## 12. Conclusion
**Find Your Home** aims to modernize the rental process in Bangladesh by providing a reliable, easy-to-use platform for tenants and house owners.  
Starting with Sylhet and Dhaka, the system will expand nationwide after successful adoption.

## 13. References: 
- [YouTube Playlist: Airbnb Clone Fullstack Tutorial](https://www.youtube.com/playlist?list=PLnE5DGXxG1AqX7BdIt_3_9RVXdDiMTAGl)  
- [GitHub Repository: Full Stack Code](https://github.com/PardeepBhasin/airbnb-clone)
