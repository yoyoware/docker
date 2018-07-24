after cloning this folder from git you will can start the container however the website will show an initial error around permissions
to solve this problem run the 'docker-compose up &'
once it runs once the 'web' folder is created
you can now stop the docker-compose with 'docker-compose down'
you will see the 'web' folder has been created
next change the mode of the folder to 777 to allow the current non root user to edit the folder content; 'sudo chmod 777 web'
next change to the web folder and edit a new index.html with the website default page content; 'cd web' 'vi index.html'
save the index.html
restart the nginx server 'docker-compose up &'

