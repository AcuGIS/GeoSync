Databases
=====

The Database page is where you can create PostGIS databases, as well as onnect to existing PostGIS databases.

Usage
------------

To create a Database, click the "Add New" button at top as show below:


   .. image:: images/add-database-1.png

For Database Type select either Local or Remote as shown below.

Local will create a PostGIS database on the GeoSync server, which you can then access.

Remote will prompt you for a remote PostGIS database that you wish to use.

   .. image:: images/admin-6.png


Populate the required fields as show below:

   .. image:: images/admin-7.png




Project:  The QGIS Project name.  This is case sensitive and must be the exact name of the QGIS Project.

Workspace:  The Workspace on your Mergin Server.  When self-hosting this value will always be "mergin".  If using Mergin Maps Team account or Enterprise Edition, this will be the actual Workspace name.

Mergin:  Select the Mergin Maps server in use from the drop-down.

GeoPackage:  This field is case sensitive and must be the exact name of the GeoPackage for the Project.  Include only the name and not the extension(.gpkg)

Password:  This will serve as the PostGIS database password.

Click the "Next" button to save the Project


Actions
------------

The Actions at right allow you to edit and delete projects, as well as show as well as dislay database connection information 

To display database connection, click on Show Connection icons as shown below:

   
   .. image:: images/project-4.png


A modal with the information will be displayed, along with a Copy button as shown below:


   .. image:: images/project-5.png


