# Venue Organizer
Team Members: Annetta Stogniew, Allison Li, Sydney Pruitt, Ania Misiorek

## Summary
For our project, we decided to create a database that manages data related to venue and event organization. Our database will allow users or attendees to schedule reservations for events. The database will also hold information related to these events, such as the performer, attendees, and time.

## UML Diagram
db_design_final_project_UML.pdf

## User Data Model
Attendees will be our user data model and they will be the users of our application. They will have a field for their first name, last name, username, password, email, and date of birth. Users will be able to make reservations for certain events.

## Domain Object 1
Event will be our first domain object. It will have a field for the room, capacity, and the date and time of the event. Events will have reservations made that represent an attendee.

## Domain Object 2
Reservations will be our second domain object. It will have a field representing the user that made the reservation and the event corresponding to the reservation.

## Domain Object 3
Performer will be our third domain object. It will have a foreign key for the event that the performer will perform in and fields for the performer’s name and genre. The genre will be a portable enumeration that has the options “comedy, music, dance, theater”. 

## User to Event Relationship
There will be a many-to-many relationship between users and events. In other words, many users will be able to attend many events. To reify this relationship, the reservation domain object will act as an intermediate relationship. Users and events will both have a one-to-many relationship with reservations.

## Event to Performer Relationship
There will be a one-to-many relationship between events and performers. In other words, one event will have many performers. 

## Portable Enumeration
Our portable enumeration will exist in the Performer domain object. Each performer will have its own genre. For example, the "comedy" enumerations will represent a comedian or comic act. Music will be an artist or band.

## User Interface Requirements
Our user interface will 
