**This is the Item Catalogue project created by Tanvir Hasan.**

Introduction:

 This project is about restaurants and their food menus. The authorized users can add, edit or delete food menu items and restaurants. Visitors can only see the restaurants and the food menu items but only an authorized person can add, edit or delete restaurants and food menu items.
           
           
Requirements:

 a. Vagrant and VirtualBox.             
 b. git.             
 c. github for desktop.             
 d. python.
       
	   
Connect with Google:

 a. First visit http://console.developers.google.com and login to your Google account.
 b. Then click 'Create project' and give a  name your project. Google will automatically create the project id.
 c. Now you will be redirected to the project dashboard.
 d. Click on 'Apis&auth' and select 'Credentials'.
 e. Then click 'Create new client ID' and select 'Web application' and then click Configure consent screen.
 f. Now in the consent screen, provide email address, product name and save changes and then click 'Create client ID'.
 g. You will get client id for the web application.
 h. Then click on download json and download the json file. Call it client_secrets.json and store in the project.
 i. Now in login.html put the client id to data-clientid = "your client id".
            
Configure your vagrant environment:

 a. vagrant init hashicorp/precise32.
 b. Use sudo apt-get install python-sqlalchemy to install sqlalchemy.
 c. Now sudo apt-get install python-pip to install pip.
 d. Finally sudo apt-get install Flask to install Flask.
 
JSON API:
 a. /restaurant/<int:restaurant_id>/menu/JSON : It provides all restaurant food menu items for the given restaurant_id.
 b. /restaurant/JSON : It provides all the restaurants.
 c. /restaurant/<int:restaurant_id>/menu/<int:menu_id>/JSON : It provides the restaurant food menu item for the given restaurant_id and menu_id.
            
Run the project in terminal:

 a. Type vagrant up.
 b. vagrant ssh.
 c. cd /vagrant (This will take you to the shared folder between your virtual machine and host machine).
 d. Now type ls to ensure that you are inside the directory that contains project.py, database_setup.py, and two directories  'templates' and 'static'.
 e. Type python database_setup.py to initialize the database.
 f. Then type python lotsofmenus.py to populate the database with restaurants and menu items. 
 g. Finally python project.py to run the Flask web server.
 h. Now in your browser visit http://localhost:5000 to view the restaurant menu app.
 

If you face any issues or want suggest me to improve the project, email to tanvir@mrsft.com

Thanks!!


