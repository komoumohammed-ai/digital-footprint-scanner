# Digital Footprint Scanner — Development Plan

## Goal

Build a full-stack application that allows users to scan their own email address and phone number for potential online exposure.

## Planned Stack

### Frontend
- React
- TypeScript

### Backend
- Java
- Spring Boot

### Database
- PostgreSQL

### Later Infrastructure
- Docker
- GitHub Actions
- AWS

### External APIs
- Have I Been Pwned
- Twilio Lookup
- Additional provider if needed

## MVP 0 — Frontend ↔ Backend

The first milestone is intentionally simple.

User enters:
- Email
- Phone number

React sends the information to:

POST /api/scans

Spring Boot receives the request and returns a fake result:

{
  "score": 67,
  "breachCount": 4,
  "emailExposed": true,
  "phoneValid": true
}

React displays the result.

### Do NOT add yet

- PostgreSQL
- External APIs
- Authentication
- Docker
- AWS
- Payments

## Future Milestones

1. Connect React to Spring Boot
2. Add PostgreSQL
3. Add real breach API
4. Add phone lookup API
5. Add testing
6. Add Docker
7. Add CI/CD
8. Deploy
9. Get real users
10. Add analytics and monetization testing