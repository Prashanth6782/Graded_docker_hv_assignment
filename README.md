
# Project Title

A brief description of what this project does and who it's for


GIT HUB link 	https://github.com/Prashanth6782/Graded_docker_hv_assignment.git


Docker compose once created was run with the below command 
docker-compose up -d
Create the below steps and I have used docker compose as well.
Basic HTML Page:
The code is there in the git repository 
2. Nginx Configuration:
   - Create an Nginx configuration file named `nginx.conf` that serves the `index.html` page.
   - Configure Nginx to listen on port 80.
3. Dockerfile:
   - Create a `Dockerfile` to define the Docker image.
   - Use an official Nginx base image.
   - Copy the `index.html` and `nginx.conf` files into the appropriate location in the container.
   - Ensure that the Nginx server is started when the container is run.
4. Building the Docker Image:
   - Build the Docker image using the `Dockerfile`.

I created an ubuntu Ec2 instance with the ARM architecture and installed the AWS CLI for the same…
Did the “aws configure” then
Finally login succeeded as shown below 
 
After saving the docker image I transferred the saved docker image to Ec2 instance via winscp as shown below 
 
Once connected to the EC2 instance, load the Docker image from the .tar file:
 
You need to tag your local Docker image with the Amazon ECR repository URI. Assuming your local image is pk1-repo:latest, you would tag it like this:
 
Verify the tagging the images 
 
Pushing the image to ECR finally 
 
Verifying the image in console (ECR) 
 
 



