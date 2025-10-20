The Airbnb Clone Project is a comprehensive, real-world application designed to simulate the development of a robust booking platform like Airbnb. It involves a deep dive into full-stack developmIIEHZfocusing on backend systems, database design, API development, and application security. This project enables learners to understand complex architectures, workflows, and collaborative team dynamics while building a scalable web application.Master collaborative team workflows using GitHub. 

Team Roles

BUSINESS A : A business analyst understands a customer's business needs and translates those needs into requirements. Also helps the product development team understand the entire business process of the busines so they can reach maximum satisfaction wth the clients
PRODUCT OWNER : A product owner is incharge of keeping the vision of the business and ensuring that at every point in the business the product developers are in line with it and at the end of the process. They are also incharge of ensuring the results are in line with the vision.
PROJECT MANAGER : A person that ensures that the product is delivered in time and on budgeet. They plan tasks and assign the tasks.
UI/UX DESIGNER : They turn the ideas or visions into user-friendly designs that align with the vision and goal of the project. They can be split into UI/UX (User Interface &User design)
SOFTWARE ARCHITECT : They design the schematics of the product and they are expert-level software engineer who makes executive software design decisions on behalf of anapp development team.
SOFTWARE DEVELOPER : Builds the product from ground up by coding the programme. They can be backend, frontend or full stack. They also ensure they also solve technical problems.
QUALITY ASSURANCE ENGINEER : Ensures an application meets all necassary requirements both functional and non functional.
TEST AUTOMATION ENGINEER : Tests the application to know that they are reliable and give continuous feedback on application quality without any human involvement.
DEVOPS ENGINEER: Facilitates cooperation between development and operations
teams and build continuous integration and continuous delivery (CI/CD)
pipelines for faster delivery.

Technology Stack

CI/CD Pipelines
Django
MySQL
GraphQL
PostgreSQL

CI/CD Pipelines: An automated process that integrates and deploys software changes.It combines Continuous Integration (CI) and Continuous Delivery (CD) to build, test, and release applications more quickly and reliably.
Django: It is a high-level Python web framework that encourages rapid development and clean pragmatic design.
MySQL: Database management system that’s used to retrieve, update, delete, and also manipulate data in relational databases.
GraphQL: An open-source data query and manipulation language for APIs and also makes it easier to aggregate data from multiple sources.
PostgreSQL: It is designed for enterprise-level performance and is valued for its robust features and reliability.

Database Design

Users
Properties
Bookings
Reviews
Payments

Users:
user id – Unique ID for each user.
name – Full name of the user.
email – Used for login and communication.
Relationships:
A user  can have multiple listings.
A user can make multiple bookings.
A user can write or receive multiple reviews.
A user can have many messages (sent and received).

Properties:
listing id – Unique ID for each property.
host id – References the user id of the host.
title – Short name of the property.
Relationships:
Each Property belongs to one host (user).
A property can have many bookings.
A property can have many reviews.
A property can have many photos and many amenities.
A prperty can appear in multiple wishlists.

Booking:
booking id – Unique booking identifier.
listing id – Property being booked.
guest id – The user making the booking.
Relationship
Each booking belongs to one listing.
Each booking is made by one guest (user).
Each booking may have one payment record.
Each booking can have one or more reviews after completion.

Review:
review id – Unique ID for the review.
reviewer id – User who wrote the review.
listing id – Property being reviewed.
rating – Numerical score (1–5).
Relationships:
A review belongs to one listing.
A review is written by one user (reviewer).
A listing can have many reviews.
A user (host or guest) can receive many reviews.

Payments:
payment id – Unique payment reference.
booking id – Booking this payment is tied to.
amount – Total amount paid.
status – Transaction result (successful, failed, refunded).
payment method – Card, PayPal, Flutterwave, etc.
Relationships:
Each payment belongs to one booking.
A booking has exactly one payment record.

Feature Breakdown

User management
Property management
Booking system
Messaging system 
Admin dashboard

User management:This feature handles user registration, authentication, and profile management. It allows users to sign up as guests or hosts, verify their identities, manage personal information, and maintain trust across the platform.
Property management: Hosts can create, edit, and manage their property listings. This includes adding photos, descriptions, amenities, pricing, and availability.
Booking system: The booking system manages reservations between guests and hosts. It handles availability checks, date selection, price calculations, and booking confirmations or cancellations
Messaging system: A built-in chat or messaging feature allows hosts and guests to communicate directly before and after booking. It supports inquiries, negotiations, and clarifications about stays.
Admin dashboard: Admins can monitor users, listings, and transactions from a centralized dashboard. It supports moderation, dispute resolution, and system oversight. This ensures platform safety, maintains quality control, and allows administrators to enforce rules and handle reports efficiently.
