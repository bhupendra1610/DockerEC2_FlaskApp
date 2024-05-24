Create an EC2 instance:<br>
	In security groups set the inbound rule:<br>
		select the custom TCP and port to be 3000
		
Connect the EC2
Write the commands:<br>

 #root user
  
 	sudo su
  
#update the shell

	yum update -y							

#install the docker

	yum install docker -y
	
#version of docker

 	docker --version	

#start the docker

 	service docker start

#status of docker

 	service docker status

#login in docker 

 	docker login

	
 #pull the repository
	
  	docker pull username/repositoryname:tag
	
eg:<br>
docker pull bhupendra16/bhupendravaishanv:latest<br>
by default tag name is latest

#view docker images

 	docker images
	
#run container

 	docker run -p containerport/tcp imageid

eg:<br>
docker run -p 3000:3000/tcp bhupendra16/bhupendravaishnav:latest

Open the ipv4 of the EC2 instance 
	http://ip:3000
