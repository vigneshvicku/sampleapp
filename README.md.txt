The SimpleTimeService is a basic Python-based web microservice that provides the current timestamp and the IP address of the client making the request
Create a file name SimpleTimeService.py and save it

Command for run the pythn script
           python3 SimpleTimeService.py 

Run the project by using docker 

Install docker(27.5.1) on the ubuntu machine
Create a group for docker
      sudo groupadd docker
      sudo usermod -aG docker $USER


1. Clone the repo and build the dockerfile
     docker build -t simple-time-service .

2. Once the Docker image is built, you can run the application in a Docker container.
     docker run -d -p 8080:8080 simple-time-service

3. After the container is running, you can access the SimpleTimeService via:
     http://localhost:8080/