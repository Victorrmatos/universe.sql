# PostgreSQL Database Dump
This repository contains a PostgreSQL database dump, which can be used to recreate a database with the same schema and data as the original database from which it was created.

Prerequisites
In order to use this dump file, you will need to have PostgreSQL installed on your system. You can download PostgreSQL from the official website.

Usage
To create a new database using this dump file, follow these steps:

Open a terminal window and navigate to the directory where you have saved this dump file.

Type the following command to create a new database from the dump file:

$ createdb -U <username> -O <username> <database_name>
$ psql -U <username> -d <database_name> -f <dump_file>
Replace <username> with the name of the PostgreSQL user who will own the new database, <database_name> with the name you want to give to the new database, and <dump_file> with the name of the dump file.

For example, if the dump file is named universe.sql, the command would be:

$ createdb -U postgres -O postgres universe
$ psql -U postgres -d universe -f universe.sql
Once the database has been created, you can connect to it using the following command:

$ psql -U <username> -d <database_name>
Database Structure
This dump file contains a PostgreSQL database with the following structure:

One database named universe.
Four tables: blackhole, galaxy, moon, and planet.
Four sequences: blackhole_blackhole_id_seq, galaxy_galaxy_id_seq, moon_moon_id_seq, and planet_planet_id_seq.

License
This repository is licensed under the MIT License.
