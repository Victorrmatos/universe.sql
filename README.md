  # PostgreSQL Database Dump
This repository contains a dump of a PostgreSQL database that includes tables for galaxies, stars, planets, and moons. 
The dump file was created with PostgreSQL version 12.9 using pg_dump.

  Usage
To use the dump file to create a new PostgreSQL database, you can follow these steps:

1 Make sure you have PostgreSQL installed on your computer.
2 Clone this repository to your local machine.
3 Open a terminal or command prompt and navigate to the cloned repository's directory.
4 Run the following command to create a new database named "universe" using the dump file:
bash
  psql -U <username> -d <database_name> -f universe.sql
Make sure to replace <username> and <database_name> with your PostgreSQL username and the name you want to give your 
new database, respectively.

  Database Tables
The dump file contains the following tables:

  blackhole: Contains information about black holes, including the black hole's ID, name, and the ID of the galaxy it belongs to.

  galaxy: Contains information about galaxies, including the galaxy's ID, name, description, number of stars in billions, 
and whether the galaxy is spherical or not.

  moon: Contains information about moons, including the moon's ID, name, radius in kilometers, whether it has life or not, 
and the ID of the planet it belongs to.

  planet: Contains information about planets, including the planet's ID, name, number of recorded moons, whether it has 
life or not, and the ID of the star it orbits.

  star: Contains information about stars, including the star's ID, name, temperature, and distance from Earth.

  License
This project is licensed under the MIT License - see the LICENSE file for details.
