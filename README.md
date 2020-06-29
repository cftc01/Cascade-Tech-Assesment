# Technical Assessment
NOTE: The majority of the work for this position will be using JS with ES6 syntax.
## Overview
Please complete this exercise with node.js and ES6. This exercise is intended to take no longer than 4 hours.  Please limit the detail of your solution with that time in mind.  Please include a README with your submission detailing your solution.

For example,
```
Do the endpoints need to be secured?  I assumed not for this exercise but would suggest adding authorization in the future.
```
## Problem
Lets assume Cascade Fintech has contracted you to build a small **RESTful API** to support their new user tracking software.  

Data does not need to be persisted between server restarts.

## Data definition

### User
- email
  - string
  - This field is required to create a new user
  - The system must only allow 1 user per unique email address
- password
  - string
  - This field is required to create a new user
- phone number
  - number
  - This field is required to create a new user
  - When provided, the phone number must follow this pattern ##########
### Event
- type
  - This field is required to create a new event
  - The value can be any non-empty string

## Data examples

The following input json would create a user
```json
{
  "email": "tester@cascadefintech.com",
  "password": "VegansRule",
  "phone": "3332221111"
}
```
___
The following input json would create an event with the type LOGIN
```json
{
  "type": "LOGIN"
}
```
___

The following use cases should be satisfied to get user event data
- return all failed login events for all users
- return all login events for a single user
- return all events for the day before last
- return all events for the week before not including session timeout

The json data returned should at least have the following elements
```json
[
  {
    "type": "LOGIN",
    "created: 47239847298347
  }
]
```
where `created` is the date the event was created.  Choose the format that works best.
___

## Submission
- Send an email to hr@cascadefintech.com with a link to your solution on your github account. Do not submit a PR. 
