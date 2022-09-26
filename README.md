# Proyecto 3

## Server

#### Endpoints

| PATH                  | METHOD | RESPONSE            | ACTION                                |
| --------------------- | ------ | ------------------- | ------------------------------------- |
| auth/signup           | POST   | 200                 | User signup                           |
| auth/login            | POST   | 200 +Object user    | User login                            |
| user/logout           | GET    | 200                 | User logout                           |
| user/delete/:id       | POST   | 200                 | User gets deleted                     |
| user/profile/:id      | GET    | 200 +Object user    | User sees its own profile             |
| user/profile/edit/:id | POST   | 200                 | User edit its own profile             |
| trip/all              | GET    | 200 +Array of trips | User(driver) sees all available trips |
| trip/new              | POST   | 200                 | User(client) creates a new trip       |
| trip/:id/driver       | PUT    | 200 + trip details  | Trip has a new driver                 |
| trip/:id/finished     | PUT    | 200                 | Trip is finished                      |

#### Models

LOOK AT THE PROJECT

## Client

#### Endpoints

| PATH                  | DESCRIPTION                                                         |
| --------------------- | ------------------------------------------------------------------- |
| /                     | Home page                                                           |
| /signup               | Signup form                                                         |
| /login                | Login form                                                          |
| /user/profile/:userid | Show profile details of user                                        |
| /user/edit/:userid    | Edit user form where user can delete or edit its own profile        |
| /user/home            | User homepage, navigate() => depends on user role(client or driver) |
|                       | if Driver list of trips                                             |
|                       | if Client map + newTrip button                                      |
| /user/trip/:tripid    | Trip data, conditional rendering if client or driver                |

#### Components list

TODO
