# Software Requirement Specifications (SRS)
### Find Your Home – Accommodation Marketplace for Tenants

## 1. Introduction

### 1.1 Purpose
The purpose of this document is to define the software requirements for **Find Your Home**, a rental accommodation platform designed to help people easily find rental homes in major cities of Bangladesh, starting with Sylhet and Dhaka.  

This README describes the system’s functionality, scope, constraints, workflow, and reference links to guide development and evaluation.

### 1.2 Problem Statement
People moving to cities like Sylhet and Dhaka struggle to find trusted rental housing options. Key issues include:

- Difficulty finding available rentals  
- Lack of verified information  
- Dependency on brokers  
- Time‑intensive physical searching  

Existing solutions lack localization for Bangladesh.  

### 1.3 Proposed Solution
**Find Your Home** is an online rental marketplace connecting:

- **Renters/Tenants**  
- **House Owners/Landlords**  

The system enables property searching, detailed viewing, authentication, booking, and interaction.  

---

## 2. Scope of the Project

### 2.1 Initial Scope
- Target service areas:  
  - **Sylhet City**  
  - **Dhaka City**  
- Accommodation types:  
  - Apartments  
  - Rooms  
  - Houses  
  - Shared accommodation  

### 2.2 Future Scope
- Nationwide expansion  
- Mobile app (React Native / Flutter)  
- AI recommendations and smart filters  
- Integrated payment system  

---

## 3. System Overview
**Find Your Home** is a web marketplace with roles:

1. **Tenant**  
2. **House Owner**  
3. **Admin**  

The app allows authenticated users to create accounts, list properties, search with filters, and manage bookings.  

---

## 4. Functional Requirements

### 4.1 Tenant Features
- Register and login (email/password)  
- Profile management  
- Search rental listings by city, area, price range, property type  
- Advanced filters (rooms, amenities)  
- View listing details: photos, price, facilities, host details  
- Booking system: select dates, check availability  
- Favorites / Wishlist  
- Booking history  

### 4.2 House Owner Features
- Owner registration & login  
- Create and manage property listings: title, description, images, price, availability  
- Update/edit/delete listings  
- View booking requests and confirm/decline bookings  

### 4.3 Admin Features
- Admin authentication  
- Approve/verify listings  
- User management: suspend or remove suspicious accounts  
- Remove fake or duplicate listings  
- Monitor site activity and analytics  

---

## 5. Non‑Functional Requirements
- **User‑Friendly UI** — intuitive front end  
- **Secure Authentication**: JWT or session-based, password hashing, optional Google OAuth  
- **Fast Search Performance**  
- **Responsive Design**  
- **Data Protection**  
- **Scalability** — support many users & listings  
- **Cross‑Browser Compatibility**  

---

## 6. Technologies Used

### 6.1 Frontend
- React.js / Next.js  
- Tailwind CSS / UI library  
- React Router  
- Axios for API calls  

### 6.2 Backend
- Node.js  
- Express.js  
- REST API  

### 6.3 Database
- MongoDB (NoSQL)  

### 6.4 Authentication
- JWT / OAuth (optional Google Auth)  

---

## 7. Dataset Description
- **Property listings**: location, price, rooms, amenities, images  
- **User data**: profile, login info (no NID/passport stored)  
- **Booking data**: dates, tenant ID, property ID  

Data can be **seeded manually for development or demo purposes**.  

---

## 8. System Workflow
1. User registers or logs in  
2. Tenant searches property listings  
3. Tenant filters and selects a property  
4. Tenant views property detail page  
5. Tenant requests a booking (date selection)  
6. Owner reviews and confirms booking  
7. Booking details are stored  
8. Tenant visits property physically and completes verification  

---

## 9. Application Architecture
- **Frontend:** React or Next.js with modern UI components  
- **Backend:** REST APIs with Express  
- **Database:** MongoDB  
- **Authentication:** JWT sessions  

---

## 10. Limitations
- No integrated online payments initially  
- No digital storage of NID/passport  
- Limited initial service area  

## 11. Revenue Model
The website owner generates revenue by monetizing the marketplace connecting **house owners** and **tenants**.

### 11.1 Commission on Bookings
- A fixed percentage of rent per booking is retained by the platform.  

| Rent (BDT/month) | Commission % | Platform Earnings (BDT) |
|-----------------|--------------|-------------------------|
| 10,000          | 5%           | 500                     |
| 15,000          | 5%           | 750                     |

**Workflow:** Tenant books → platform deducts commission → remaining rent goes to owner → commission retained by platform.

### 11.2 Featured Listings / Premium Placement
- Owners can pay to highlight their property or appear on top of searches.  
- Example: BDT 200–500 per listing per month  

### 11.3 Subscription Model (Optional / Future)
- Premium features for tenants or owners (AI recommendations, unlimited listings, analytics dashboards)  

### 11.4 Advertisements
- Local businesses (furniture, moving services, cleaning) can advertise on the platform  
- Example: BDT 500–1,000 per ad per month  

### 11.5 Optional Add-ons
- Booking protection / security deposit handling  
- Cancellation fees  
- Premium support services  

### 11.6 Revenue Flow
1. Tenant books → payment via gateway → commission deducted → balance to owner  
2. Featured listings, subscriptions, ads → collected directly by platform  
3. Payments processed via gateways (bKash, Nagad, Rocket, SSLCommerz, Stripe)  

**Expected Revenue Example:**  
- 1,000 listings × 5% commission × avg. rent BDT 10,000 = BDT 500,000/month  
- Expansion to 10 cities → potential revenue = BDT 5,000,000/month  
- Additional revenue from featured listings & ads = BDT 200,000–500,000/month  

## 12. Conclusion
**Find Your Home** is a web application to modernize the rental search process in Bangladesh, with core features inspired by full‑stack Airbnb clone tutorials. It delivers authenticated workflows for tenants and owners, scalable design, and usable interfaces — preparing it for future enhancements like mobile apps and AI-based recommendations.

## 13. References
- [YouTube Playlist: Airbnb Clone Fullstack Tutorial](https://www.youtube.com/playlist?list=PLnE5DGXxG1AqX7BdIt_3_9RVXdDiMTAGl)  
- [GitHub Source Code](https://github.com/PardeepBhasin/airbnb-clone)
