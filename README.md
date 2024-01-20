# EC2 Sandbox

## Exercise: Setting up AWS EC2 using terraform
This is an exercise to setup AWS EC2 using terraform. 
- Perform setup using terraform

## Exercise: Deploying python flask app using docker onto AWS EC2
Prerequisites: 
- AWS EC2 (created using terraform)
- Run ```sudo yum install docker -y``` and ```sudo yum install git -y``` on AWS EC2 to install docker and git. 

### Using docker to launch application
1. Connect to your EC2 using SSH client. 
2. In your EC2 terminal, clone current repo using ```git clone https://github.com/coolkiddzzz/first-docker-exercise.git```
3. Run docker as root user (using ```sudo -i```)
4. Use docker to create docker image using ```docker build -t first-docker-exercise /home/first-docker-exercise/.```
5. Start docker container using ```docker run -d -p 5000:5000 <image-name>```

## Exercise: Create a Simple EC2 Web Server with Apache
1. Install apache web server ```sudo yum install -y httpd``` in AWS EC2
2. Start apache service using ```sudo systemctl start httpd```
3. Clone repo into /var/www/html using ```git clone https://github.com/coolkiddzzz/first-docker-exercise.git /var/www/html```
4. Access web server from public IP

## Other Ideas 

