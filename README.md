# Local Government Units in Luzon
Philippines' Local Government Units in Luzon
(github.com/mksalada/LuzonLGUs)

# About This Application:
This web application manages the data of the Local Government Units (LGU) in the Philippines but only covers the regions of Luzon island: National Capital Region (NCR), Regions 1 to 5, and Cordillera Administrative Region (CAR). This application is inspired from the Local Government Academy's Local Government Units Directory (lga.gov.ph/directory) where you can find all of the LGUs in the whole Philippine islands.

The database was made easy because of OJ Tibi's Philippine Provinces and Cities database (bit.ly/2sjMM8Y) and the Wikipedia maps of the LGUs from Local Government Academy website.

# Installation Materials:
Text editor, Web browser, Web server, Database application

# Installation Procedures:
First, ensure that your web server's Apache and MySQL are both running. Then, import the "luzonlgus.sql" script in your database application inside your choosen database.

Copy the "lgus" folder inside your web server's "www" or "htdocs" folder. Then, open it. You will see a folder named "public". Copy it's location address.

Inside your web server's Apache folder, open the "httpd.conf" file in your text editor. Find "DocumentRoot", paste the "public" folder's location as replacement to its default address. Do it also on "Directory" address under it. Just like this:

        DocumentRoot "${INSTALL_DIR}\www\lgus\public"
        <Directory "${INSTALL_DIR}\www\lgus\public">

Then, inside the "lgus" folder, open the folder named "app", and open the "database.php" file in your text editor. Find the "class Database" and inside it, find "public $default". Change the "hostname", which is "localhost" if you want, and provide a "username", "password" (you can leave this blank) and "database".
Now open your web browser and type "localhost".

# For inquiries, go to this link -> https://mksit.tk/lgusph/about.html#contact.
