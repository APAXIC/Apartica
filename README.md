# Apartica

**Apartica** is a full-stack accommodation booking platform for short-term stays. It connects guests looking for accommodation with property owners who publish listings, manage availability-related booking activity, and receive reservations through the platform.

The application supports four user roles – guest, property owner, moderator, and administrator – with different workflows and permissions. It brings together property listings, location-based discovery, image management, online payments, reviews, and content moderation.

## Features

- **Role-based functionality:** Separate workflows for guests, property owners, moderators, and administrators.
- **Authentication:** User sign-in with JWT-based authentication and Google OAuth 2.0 integration.
- **Property owner registration:** A dedicated registration flow for users who want to publish accommodation.
- **Email verification:** Send registration confirmation codes to users via the SendGrid API.
- **Accommodation listings:** Owners can submit properties and rooms with descriptions, locations, and required photographs.
- **Google Maps integration:** Select a property's location by address when creating a listing and view its location when browsing accommodation.
- **Media management:** Upload and manage photographs of properties and rooms.
- **Property and booking management:** Owners can manage their listings and review bookings made for their accommodation.
- **Accommodation discovery:** Guests can search and filter listings, inspect property details, and explore locations on a map.
- **Booking and payments:** Reserve a property or room and complete payment through Stripe API integration.
- **Booking confirmation emails:** Notify users by email when their bookings are confirmed, using SendGrid.
- **Guest reviews:** Leave accommodation reviews after a completed booking and stay.
- **Content moderation:** Moderators review requests to publish new properties and reviews, approving or removing submissions.
- **Administration:** Administrators can perform CRUD operations on most application entities.

## Tech Stack

| Layer | Technology |
| --- | --- |
| Backend | JavaScript, Node.js, Express.js |
| Frontend | JavaScript, React |
| Database | MongoDB, MongoDB Atlas |
| Data access | Mongoose |
| Authentication | JWT, Google OAuth 2.0 |
| Payments | Stripe API |
| Maps and location | Google Maps API |
| Transactional email | SendGrid API |
| Hosting | Render (used for deployment) |

## How It Works

Apartica uses a client–server architecture with role-specific application flows:

1. **Guests** search for accommodation, filter results, inspect property details and map locations, and book properties or rooms using Stripe-powered payments.
2. **Property owners** complete a dedicated registration process, submit listings with locations and photos, and manage their properties and bookings.
3. **Moderators** review publication requests for new accommodation and guest reviews.
4. **Administrators** manage most application entities through CRUD operations.
5. **Email notifications** use SendGrid to deliver registration verification codes and booking confirmation messages.
6. **Express.js backend** coordinates application requests, authentication, booking operations, and integrations with external services, while MongoDB stores application data through Mongoose.

Google Maps supports address-based location selection and property location display. Stripe handles the payment integration for reservations, Google OAuth 2.0 provides an additional authentication option, and SendGrid delivers transactional emails.

## Availability

A public deployment is not currently available.

## Author

- **Andrii Vus**  
  GitHub:  https://github.com/APAXIC  
  LinkedIn:  https://www.linkedin.com/in/andrii-vus/  
  Email:  irishardron@gmail.com