My Person class might hold the following fields:

id - user ID
firstName (String) - user’s first name
lastName (String) - user’s last name
email (String) - user’s email
password (String) - user’s password
location (String) - user's location (city, state selection option)
age (Int) - user's age

The class would need getters for all of these fields. It could have setters for all fields except id (since it shouldn’t change).

The Person class might also have the following references:

Profile - a class to gather up all of the profile information about the user
List<ActivityCategories> categoriesInterested - to store categories of activities the user is interested in
List<Events> eventsAttending - a different list, to store the events the user has decided to attend
Person would have a many-to-many relationship with Events via List<Events> eventsAttending. It would have a one-to-many relationship with ActivityCategories via List<ActivityCategories> categoriesInterested.# CodingEventsJava
