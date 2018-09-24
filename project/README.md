# Practical Section (weekend project)

You are to build a scheduling system (similar to the one specified in the long answer section).

You are allowed to use _any framework/language/technology_ you like.

Your time limit is 2 days, or over a weekend.

**Requirements**: You must use a relational database.

_Bonus_: Generate a swagger document (this must be generated)

# Application Design

Given the following requirements, design an API and database schema for a scheduling system.

## User Stories

- User should be able to create, read, update and delete shifts
- User should be able to schedule workers in shifts
- User is able to view a week’s worth of shifts at a time
- User should be able to “publish” an entire week’s worth of shifts at a time
- User should not be able to edit or delete a shift after it’s been “published”
- User should not be able to create shifts in a “week” that is “published”

## Requirements

The schema should be presented as a UML class diagram (or do your own diagrams, as long as we can make sense of it). Things that should be included

- List of properties/fields for each class
- Relationships between each class

The API can be presented in bullet point form. Things that should be included

- Endpoints (and how to call/interact with the endpoint)
- Internal logic of each endpoint
