# EC2 Sandbox

## Deploying python flask app using docker onto AWS EC2
This is an exercise deploying an app using docker onto AWS EC2. 

### Prerequisites
- AWS EC2 
- Run ```sudo yum install docker -y``` and ```sudo yum install git -y```, and this will install docker and git on your EC2. 

### Using docker to launch application
1. Connect to your EC2 using SSH client. 
2. In your EC2 terminal, clone current repo using ```git clone <url>```
3. Run docker as root user (using ```sudo -i```)
4. Use docker to create docker image using ```docker build -t first-docker-exercise /home/first-docker-exercise/.```
5. Start docker container using ```docker run -d -p 5000:5000 <image-name>```


## Improvements 
- Create aws ec2 using terraform 
- Create a Simple EC2 Web Server with Apache

