# **Skyser**


Skyser is an online flight-sharing service. Its website connects pilots of varying degrees of experience with passengers wanting to travel to a common destination. The platform allows both pilots  and passengers to share the flight-related costs involved in air travel.

## Flight-sharing service
Members :
```
Oussama Aouessar
Quentin Fritz
Dalya Furaiji
Tahar Haddad
Ouriel Haddouk
Lilya Melila
Fabiana Montiel
Viviana Montiel
Sahana Sivakumaran
Nabil Zerzeri
```


## Users

| Pilot | Passenger | Guest
|--|--|--|
| The pilot will be able to add and modify their flights. The website will be available to them in order to manage their flights. They will have access to some of the passengers’ information and can thus accept or deny their request to be on the flight. | The passenger can only use the website for browsing and booking purposes. They can create an account and also access information regarding the flights and the pilots. | The user, while not yet signed up, can only search and consult future flights. The website will allow them access to flight details as well as the pilot’s basic information.|
||||

## Business objects

| Flight | Pilot | Passenger
|--|--|--|
| ID Flight | ID Pilot | ID Passenger
| ATC Number | First Name | First Name
| Departure Location | Last Name | Last Name
| Arrival Location | Email | Email
| Departure Date | Phone Number | Phone Number
| Arrival Date | Home Address | Home Address
| Departure Time | Billing Information | Billing Information
| Arrival Time | License |
| Number of Seats | Experience Hours |
| Meeting Point |  | |


## Architecture
![enter image description here](https://i.imgur.com/hSGICnD.png)


## Navigation diagram

![enter image description here](https://imgur.com/NP7Kkqp.png)

## Backlog

![enter image description here](https://imgur.com/hk6odeW.png)

## web services

 
| type | url | behavior |
|--|--|--|
| GET | /flights_list | returns the list of flights from a search
| GET | /flights_list/flight_summary/{id} | returns details of flight with the corresponding “id”
| POST | /sign_up | creates a new user (passenger)
| POST | / | verifies the users login information
| POST | /add_flight | creates a new flight
| POST | /flights_list/flight_summary/{id} | makes reservation of a flight with the corresponding “id”
| PUT | /profile/upgrade | makes the passenger into a pilot
| DELETE | /profile/settings | deletes account of a registered user
| DELETE | /flights_list/flight_summary/{id} | deletes a flight with the corresponding “id”
| DELETE | /upcoming/flight_summary/{id} | deletes a booked flight with the corresponding “id”


