OSM PostGIS
==========

This is a ready-to-go TileMill project to get you started using PostGIS with TileMill in Windows.  This project assumes that you have:

- a PostGIS database set up
- OSM data imported into the database using osm2pgsql (version 0.69)
- TileMill installed

This project is based on the OSM Bright project, but with fixes to make it work correctly with Windows.  The SQL queries contained are suited for the database structure prepared by the current version of osm2pgsql for Windows (0.69).

To get started, copy this directory into your TileMill projects folder.  This is most probably *~/Documents/MapBox/projects*.

Before opening the project in TileMill, you need to change the settings to connect to your database.  Open the **project.mml**  file with a text editor.  Use find & replace to change the database settings.  The current settings are:

	"dbname": "gisdb",
	"user": "postgres",
	"password": "pg_pass"

To change these, use find & replace to replace *gisdb* with your database name, *postgres* with your user name, and *pg_pass* with your password.

When you are finished, save the file.  Now, when you open the project in TileMill, it should load correctly.  Note that it may take a few minutes to load the first time you open the project.