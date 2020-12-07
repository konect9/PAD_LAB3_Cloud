# PAD_LAB3_Cloud
Uploading API to Cloud using Docker Container

To implement this API into Cloud, i've configured a Server using DigitalOcean.
On my server i've installed and configured Docker

Next step is to create a Dockerfile which is the script for Docker to install my project on the server.

docker-commit.yml is another file that should be written. This is a set of instructions for Docker, to know what services should be installed in order for your project to run.
It installs MongoDB and the project files of the API. Also, it configures a UI- Mongo Express wich shows the database's contents. 

Using FTP i've transfered all the project files to the server including the docker-commit.yml file.

On the server, run:
  docker-commit up -d 
This command will run the script and will install the project on the server (virtual machine)

To access the API use the following link:

http://167.99.86.115:5000/api/Todos

To make the API more friendly, i've implemented Swagger, wich is a UI used to work with API's methods.

To access the Swagger interface use the following link:
http://167.99.86.115:5000/swagger/index.html




