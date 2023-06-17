# rtcampAssignment

1. In this first file i have to Check if docker and docker-compose is installed on the system using commands.
docker --version, docker-compose --version
If not present, install the missing packages that i have added in the first file.


2. In second file i created a WordPress site using the latest WordPress version 
Create a new file called create_wordpress_site.sh and open it for editing .
And i made the script executable by running the following command:
chmod +x create_wordpress_site.sh
./create_wordpress_site.sh mysite
It is a LEMP stack running inside containers (Docker) and a docker-compose file is present.


3. Here i Created a /etc/hosts entry for example.com pointing to localhost
After running the script, we can access the WordPress site by visiting http://example.com:8000 in web browser.


4. Here i have Prompted the user to open example.com in a browser if all goes well and the site is up and healthy.
The script will start the Docker containers, add the /etc/hosts entry, and display the prompt message. The user can then manually open http://example.com:8000 in their browser to access the WordPress site.


5. In this file i have Added another subcommand to enable/disable the site (stopping/starting the containers)
To create and start the WordPress site: ./create_wordpress_site.sh example.com start
To stop the WordPress site (previously created): ./create_wordpress_site.sh example.com stop
To create the WordPress site without starting it: ./create_word


6.Here in this file i added one more subcommand to delete the site (deleting containers and local files).
If the subcommand is start, it starts the Docker containers and prompts the user to open http://example.com:8000 in the browser. If the subcommand is stop, it stops the Docker containers and displays a success message. If the subcommand is delete, it stops the Docker containers, removes the local files for the WordPress site, and displays a success message.
