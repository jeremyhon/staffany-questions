# Application Design (2 hours)

Given the following requirements, design an API and database schema for a scheduling system.

## Requirements/User Stories

- User should be able to create, read, update and delete shifts
- User should be able to schedule workers in shifts
- User is able to view a week’s worth of shifts at a time
- User should be able to “publish” an entire week’s worth of shifts at a time
- User should not be able to edit or delete a shift after it’s been “published”
- User should not be able to create shifts in a “week” that is “published”
- The entire system is constrained by a “roles” system. Workers are assigned roles, and can only be assigned to shifts that allow these roles
- User should not be able to schedule a worker if they are already allocated a clashing shift
- User should be able to modify a scheduled worker’s start time and end time without affecting the timing of other workers in the shift
- User is able to swap two scheduled workers with the same constraints as per normal scheduling (i.e. they cannot swap if one of the workers has a clashing shift)

## Optional Component (Availabilities)

- User is able to create, read, update and delete a worker’s availability for each shift
- User should only be able to schedule a worker if they are available for a shift

## Deliverables

The schema should be presented as a UML class diagram (or do your own diagrams, as long as we can make sense of it). Things that should be included

- List of properties/fields for each class
- Relationships between each class

The API can be presented in bullet point form. Things that should be included

- Endpoints (and how to call/interact with the endpoint)
- Internal logic of each endpoint
