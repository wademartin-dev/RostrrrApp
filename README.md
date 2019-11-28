# RostrrrApp

Staff scheduling web application. JAM Stack: Next.js, GraphQL (Prisma, GrapQL Yoga, Apollo).

## Data Structure

   User - 
   Business -
   Location - 
   Department
   "Team"
   "Schedule"
   "ScheduleOptions"

   Business Admin(User) -> Business -> Location(s) -> Department(s) -> Team(s) -> Schedule -> Team Members(Users)
   
## Permissions
   Permissions will be specified for each user to grant or restrict access to application funtionality. These permissions are    broken down a follows:  
   
   1. Business Admin - Full access to add and edit all Business, Location, Department, Team, and Schedule data. Able to edit Schedule Options for each team. Able to onboard new team members for all business teams accross all business locations and departments. Able to edit user permission levels for all team members within the business. Able to access chat groups for all Locations, Departments and Teams. If required can view chat transcript for user -> user chat instances for all business Locations, Departments and Teams.
   
   2. Location Admin - Full Access to create and edit location, department, team and schedule data for specified location/s where access has been granted by a Business Admin. Able to onboard new team members for all location teams accross all loaction departments. Cannot set user permission above own permisson level (i.e. cannot set a team members permission level to Business Admin).
   
   3. Department Admin - 



## Functionality

1. To begin a user must sign up (using Auth0). This requires:  
   i) A first name.  
   ii) A unique email address.  
   iii) A password.  
   iv) Alternatively 3rd party sign up may be used (Google or Facebook).

2. Once signed up the user may join an existing business (via an invite) or create a new business.

3. If the user creates a new business they must provide:  
   i) The business name.  
   ii) A unique email address.  
   iii) The business location (City, State, Country and Postcode @ minimum).

4. This business location data will be used to scaffold a single default location for the business.  
   i) The user may edit this location data as required.  
   ii) The user may add multiple locations.

5. Each time a location is created (either the default business location or user created) this cascades creation of default location data such as departments and teams.

6. Anytime following completion of step 3 the user may begin editing location data (i.e. Department and Team names), onboarding team members and creating rosters.

7. 
