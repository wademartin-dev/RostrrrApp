# RostrrApp

Staff scheduling web application. JAM Stack: Next.js, GraphQL (Prisma, GrapQL Yoga, Apollo)

## Functionality

1. To begin a user must sign up (using Auth0). This requires:
   i: A first name.
   ii: A unique email address.
   iii: A password.
   iv: Alternatively 3rd party sign up may be used (Google or Facebook)

2. Once signed up the user may join an existing business (via an invite) or create a new business.

3. If the user creates a new business the must provide:
   i: The business name.
   ii: A unique email address.
   iii: The business location (City, State, Country and Postcode @ minimum).

4. This business location data will be used to scaffold a single default location for the business.
   i: The user may edit this location data as required.
   ii: The user may add multiple locations.

5. Each time a location is created (either the default business location or user created) this cascades creation of default location data such as departments and teams.

6. Anytime from #3 the user may begin editing location data (i.e. Department and Team names), onboarding team members and creating rosters.
