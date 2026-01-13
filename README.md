Software Requirement Specification (SRS)
Project Title: Find Your Home – Accommodation Marketplace for Tenants
1. Introduction
1.1 Purpose
The purpose of this document is to define the software requirements for Find Your Home, a rental accommodation platform designed to help people easily find rental homes in major cities of Bangladesh, starting with Sylhet and Dhaka. This SRS describes the system’s functionality, scope, constraints, workflow, and revenue model to guide development, evaluation, and business planning.
1.2 Problem Statement
People moving to cities like Sylhet and Dhaka struggle to find trusted rental housing options. Key issues include:
Difficulty finding available rentals
Lack of verified information
Dependency on brokers
Time‑intensive physical searching
Existing solutions lack localization for Bangladesh
1.3 Proposed Solution
Find Your Home is an online rental marketplace connecting:
Renters/Tenants
House Owners/Landlords
The system enables property searching, detailed viewing, authentication, booking, and interaction, streamlining the rental process and reducing reliance on brokers.

2. Scope of the Project
2.1 Initial Scope
Service Areas:
Sylhet City
Dhaka City
Accommodation Types:
Apartments
Rooms
Houses
Shared accommodation
2.2 Future Scope
Nationwide expansion
Mobile app (React Native / Flutter)
AI recommendations and smart filters
Integrated payment system

3. System Overview
Roles in the system:
Tenant
House Owner
Admin
Functionalities include account creation, property listing, search with filters, booking management, and admin verification.
4. Functional Requirements
4.1 Tenant Features
Register and login (email/password)
Profile management
Search rental listings: city, area, price, property type, amenities
View listing details: photos, price, facilities, host details
Booking system: date selection, availability check, wishlist/favorites
Booking history
4.2 House Owner Features
Owner registration & login
Create and manage property listings: title, description, images, price, availability
View booking requests: confirm/decline bookings
4.3 Admin Features
Admin authentication
Approve/verify listings
User management: suspend/remove suspicious accounts
Monitor site activity and analytics

5. Non‑Functional Requirements
User‑Friendly UI
Secure Authentication (JWT or session-based; password hashing; optional OAuth)
Fast Search Performance
Responsive Design
Data Protection
Scalability
Cross‑Browser Compatibility

6. Technologies Used
6.1 Frontend
React.js / Next.js
Tailwind CSS / UI library
React Router
Axios for API calls
6.2 Backend
Node.js
Express.js
REST API
6.3 Database
MongoDB (NoSQL)
6.4 Authentication
JWT / OAuth (optional Google Auth)

7. Dataset Description
Property listings: location, price, rooms, amenities, images
User data: profile, login info (no NID/passport data)
Booking data: dates, tenant ID, property ID
8. System Workflow
User registers or logs in.
Tenant searches property listings.
Tenant filters and selects a property.
Tenant views property details.
Tenant requests a booking (date selection).
Owner reviews and confirms booking.
Booking details are stored.
Tenant visits property physically and completes verification.

9. Application Architecture
Frontend: React or Next.js with modern UI components
Backend: REST APIs with Express
Database: MongoDB
Authentication: JWT sessions

10. Limitations
No integrated online payments initially
No digital storage of NID/passport
Limited initial service area
11. Revenue Model
11.1 Revenue Generation
Revenue will be generated through multiple channels:
Booking Commission:
A fixed percentage (e.g., 5–10%) of each confirmed booking fee from the property owner.
Example: If a rent is BDT 10,000/month and commission is 5%, we earn BDT 500.
Featured Listings / Premium Services:
Owners can pay extra to highlight their property, appear on top of searches, or access analytics.
Advertisements:
Local businesses or services (furniture, moving, home services) can advertise on the platform.
Subscription Model (Optional Future):
Tenants or owners can subscribe for premium features (AI recommendations, unlimited listings).
11.2 Revenue Collection
Payments will be collected through trusted online gateways (bKash, Nagad, Rocket, SSLCommerz, Stripe).
Property owners or tenants pay commissions and fees via the platform.
Payment gateways process transactions securely and provide confirmation receipts.
11.3 Revenue Flow
User makes payment → via online gateway integrated into the platform.
Payment gateway deducts service charges → sends net amount to our platform account.
Platform records revenue → admin panel tracks earnings per booking/listing.
Owner/Tenant payments handled → commission retained by platform; balance goes to owners if applicable.
Expected Revenue:
Assuming 1,000 listings per city and 5% commission on average BDT 10,000 rent/month:
Revenue per month per city = 1,000 × 10,000 × 5% = BDT 500,000
With expansion to 10 cities, potential monthly revenue = BDT 5,000,000
Additional revenue from featured listings & ads could add BDT 200,000–500,000/month initially.
Note: Revenue is scalable with user base growth, number of listings, and future monetization services.

12. Conclusion
Find Your Home is a web application designed to modernize rental housing search in Bangladesh. It delivers authenticated user workflows for tenants and owners, scalable design, and usable interfaces for property browsing and bookings. The platform is prepared for future enhancements like mobile apps, AI-based recommendations, and monetization strategies. The revenue model ensures sustainable business growth while providing a trusted rental ecosystem.
13. Reference
YouTube Playlist: Airbnb Clone Fullstack Tutorial
GitHub Source full stack Code: GitHub Repository


