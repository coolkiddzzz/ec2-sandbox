# EC2 Sandbox

## Exercise: Initialise AWS EC2 using terraform
- Perform setup using terraform
- Perform ```terraform destroy``` after completing using EC2. 

## Exercise: Deploying python flask app using docker onto AWS EC2
Prerequisites: 
- AWS EC2 (created using terraform)
- On your EC2, run ```sudo yum install docker -y``` and ```sudo yum install git -y``` to install docker and git. 

Using docker to launch application:
1. Connect to your EC2 using SSH client. 
2. In your EC2 terminal, clone current repo using ```git clone https://github.com/coolkiddzzz/first-docker-exercise.git```
3. Check docker is installed: ```sudo -i docker --version```
4. Create docker image: ```sudo docker build -t first-docker-exercise /home/first-docker-exercise/.```
5. Start docker container: ```sudo docker run -d -p 5000:5000 <image-name>```

## Exercise: Create a Simple EC2 Web Server with Apache
1. In EC2, install apache web server ```sudo yum install -y httpd```
2. Start apache service: ```sudo systemctl start httpd```
3. Clone repo into /var/www/html: ```git clone https://github.com/coolkiddzzz/first-docker-exercise.git /var/www/html```
4. Access web server from public IP

## Other Ideas 

