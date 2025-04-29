# 🏡 Airbnb Clone Project

## 📌 Overview

The Airbnb Clone Project is a real-world, full-stack web application designed to simulate a robust booking platform like Airbnb. It offers learners hands-on experience in backend architecture, API development, database design, and DevOps practices. This collaborative project emphasizes building secure, scalable, and maintainable systems.

## 🎯 Project Goals

- **User Management:** Secure registration, authentication, and profile handling.
- **Property Management:** Create, update, and retrieve property listings.
- **Booking System:** Enable property bookings with full CRUD operations.
- **Payment Processing:** Handle transactions and track payment history.
- **Review System:** Allow users to post and manage property reviews.
- **Performance Optimization:** Use indexing and caching for improved data access.

## 🛠️ Technology Stack
- **Django:** A high-level Python web framework for building RESTful APIs and backend logic.
- **Django REST Framework (DRF):** Extends Django to simplify the creation and management of RESTful APIs.
- **PostgreSQL:** A powerful relational database used to store and manage structured data.
- **GraphQL:** A flexible query language for efficiently retrieving and modifying backend data.
- **Celery:** Handles asynchronous tasks such as notifications and payment processing.
- **Redis:** Provides caching and task queuing support for performance improvements.
- **Docker:** Offers consistent environments for development and production using containers.
- **GitHub Actions:** Automates testing, building, and deployment via CI/CD pipelines.


## 🗝️ Database Design

### 1. **User**
- **Fields:** `id`, `name`, `email`, `password`, `role`
- **Relationships:**
  - A user can own multiple properties.
  - A user can make multiple bookings.
  - A user can write multiple reviews.

### 2. **Property**
- **Fields:** `id`, `title`, `description`, `location`, `owner_id`
- **Relationships:**
  - A property belongs to a user (owner).
  - A property can have multiple bookings.
  - A property can have multiple reviews.

### 3. **Booking**
- **Fields:** `id`, `user_id`, `property_id`, `check_in`, `check_out`
- **Relationships:**
  - A booking is made by a user.
  - A booking is for a specific property.
  - A booking may have an associated payment.

### 4. **Review**
- **Fields:** `id`, `user_id`, `property_id`, `rating`, `comment`
- **Relationships:**
  - A review is written by a user.
  - A review is associated with a property.

### 5. **Payment**
- **Fields:** `id`, `booking_id`, `amount`, `payment_method`, `status`
- **Relationships:**
  - A payment is linked to a specific booking.


## 👥 Team Roles

- **Software Architect:** Designs the system architecture, selects the tech stack, and ensures code quality through standards and reviews.
- **Software Developer:** Implements the application features. Frontend developers handle the user interface, while backend developers manage logic, algorithms, and data flow. Full-stack developers do both.
- **Database Administrator (DBA):** Designs, implements, and manages the database system. Ensures data integrity, optimizes query performance, handles backups, and manages indexing and schema updates.
- **QA Engineer:** Ensures the application meets all functional and non-functional requirements through various testing types and documentation.
- **Test Automation Engineer:** Builds test scripts and automation frameworks to streamline the testing process and provide rapid feedback on application stability.
- **DevOps Engineer:** Bridges development and operations, builds CI/CD pipelines, and ensures efficient, stable, and automated deployment workflows.

## 📚 Documentation

- REST APIs follow the **OpenAPI standard** for clear and consistent documentation.
- GraphQL API supports flexible and efficient data querying.

---

> This project is a part of the ALX Software Engineering curriculum and serves as a platform to practice real-world software development principles with teamwork, planning, and deployment at its core.
