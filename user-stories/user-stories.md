# User Stories for ALX Airbnb Clone Project

This document outlines the key user stories for the Airbnb Clone project, following the "As a [role], I want to [action] so that [benefit]" format.

## Table of Contents

1. [Authentication](#authentication)
2. [Property Management](#property-management)
3. [Booking System](#booking-system)
4. [Payment Processing](#payment-processing)
5. [Reviews & Ratings](#reviews--ratings)
6. [Admin Features](#admin-features)

---

## Authentication

### US-01: User Registration

**As a** new user,  
**I want to** register as either a guest or host with my email and password (or via OAuth),  
**so that** I can access the platform's features tailored to my role.

**Acceptance Criteria:**

- Form validates email format and password strength
- OAuth options (Google/Facebook) work without errors
- Role selection (guest/host) is mandatory

### US-02: User Login

**As a** registered user,  
**I want to** log in using my credentials or OAuth provider,  
**so that** I can access my account securely.

---

## Property Management

### US-03: Create Property Listing

**As a** host,  
**I want to** create a property listing with details (title, description, price, amenities),  
**so that** guests can discover my property.

**Acceptance Criteria:**

- Required fields must be validated
- Photos upload to AWS S3
- Preview functionality before publishing

---

## Booking System

### US-04: Search & Book Properties

**As a** guest,  
**I want to** search properties by filters and book available dates,  
**so that** I can reserve a suitable stay.

**Acceptance Criteria:**

- Real-time availability checking
- Prevent double-booking
- Booking confirmation notification

---

## Payment Processing

### US-05: Secure Payment

**As a** guest,  
**I want to** pay for bookings via Stripe/PayPal,  
**so that** my reservation is confirmed instantly.

**Acceptance Criteria:**

- PCI-compliant payment processing
- Email receipt generation
- Failed payment handling

---

## Reviews & Ratings

### US-06: Submit Review

**As a** guest,  
**I want to** review properties after my stay,  
**so that** I can share my experience.

**Acceptance Criteria:**

- Only allowed for completed stays
- Star rating system (1-5)
- Host response capability

---

## Admin Features

### US-07: Manage Users

**As an** admin,  
**I want to** view and moderate user accounts,  
**so that** I can maintain platform safety.

**Acceptance Criteria:**

- Role-based access control
- Bulk action capability
- Audit logging

---
