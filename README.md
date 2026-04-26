# EGR_115_Group_Project_2

CUSTOM FLIGHT
ANALYZER
Group Members
Sam Steadman, César Battistini, Delmer J. Camp, Mckenzie Carr, Chase Lang, Blake
Washington
Project Overview
The CUSTOM FLIGHT ANALYZER has two separate, informative plots ‘Fuel
Consumption’ based on ‘Flight Time’ and ‘CO2 Emissions per Person’ based on ‘Max
Number of People on Board’ for these planes:
1) Boeing 737-800
2) Airbus A320
3) Boeing 777
4) Gulfstream G650
5) Cessna 172
For these airports:
1) Phoenix Sky Harbor International Airport (PHX)
2) Los Angeles International Airport (LAX)
3) John F. Kennedy International Airport (JFK)
4) Miami International Airport (MIA)
5) Seattle–Tacoma International Airport (SEA)
6) User Inputted Location
To calculate distance between two coordinate points, we use the Haversine formula.
This formula calculates the great-circle distance between two points given the longitude
and latitude in radians. The outputs for the formula are based on the units provided for
the radius; we used nautical miles in our code. The biggest highlight of this project
would be the advanced use of dictionaries for easy access of information later in the
code. It also allows the code to be super modular so that new locations or planes can be
more easily added.
Features
As mentioned above, the code, given the user inputs, can calculate the fuel burned,
pollution produced, and time allotted based on coordinate locations. These are
calculated based on distance between locations, fuel efficiency in gallons per hour, and
cruising speed in knots. The code also allows for the user to input a unique location of
their choice. At the start, the user is prompted 'YES or NO - Would you like to select a
stored location?' and, if ‘NO’ is inputted, the user is then asked to provide a name,
longitude coordinates, and latitude coordinates for their desired location. The code does
this inside of a while loop and returns 'Error - Please select either YES or NO' if neither
‘YES’ or ‘NO’ is inputted. This loop only breaks once one of those is selected.
Example Code Flow Upon Start:
Output 1: ‘YES or NO - Would you like to select a stored location?’
User input: ‘no’
Output 2: 'Error - Please select either YES or NO'
‘YES or NO - Would you like to select a stored location?’
Assuming the user has selected ‘YES’, the code will either ask them to provide the name
of the airport they wish to select and run all the calculations from there. Once again, if
the user does not provide a designated string value, the code will return an error and
have them repeat their code.
Example Code Output
Physics Model
While we do not have a very advanced model, we do have an easy to use,
basic, reliable model that is only a few percent off of what we would truly
find it to be in real life. The most complicated component is the Haversine
formula; this however is still slightly off as it does not, and cannot, account
for the slightly oblong nature of the Earth.
Time = Distance / plane.speed
Fuel Consumed = Time * plane.EFF
