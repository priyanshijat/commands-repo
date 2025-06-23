```
sudo apt update
```
to update

```
vi jenkins.sh 
```
```
#!/bin/bash

# to install java
sudo apt update
sudo apt install fontconfig openjdk-21-jre -y

# installation of jenkins
sudo wget -O /etc/apt/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
echo "deb [signed-by=/etc/apt/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins -y
```
to install jenkins in ubuntu linux

```
sudo apt install docker.io -y
```
to install docker

```
sudo usermod -aG docker ubuntu
sudo usermod -aG docker jenkins
```
to add ubuntu and jenkins in docker group 

add 8080 in your ec2 instance security group


