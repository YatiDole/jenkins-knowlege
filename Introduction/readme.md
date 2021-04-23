# Introduction

## What is jenkins?
	* Open-source CI?CD tool written in java.
	* Jenkins is forked from Hudson.
	* It is a server based application which requires web-server like Apache Tomcat.

## Why use Continuous integration with Jenkins?
	* Using jenkins code is built and tested as soon as developer commits code.
	* On successful Build Jenkins will deploy the source code to Test server and notifies Dev Team.
	
## Advantages of Jenkins
	* Jenkins managed by community:-Active builds
	* Jenkins supports cloud based architectureso that you can deploy Jenkins to cloud-based platform.
	* We can containerize Jenkins service. (eg. Docker)
	
## Jenkins Alternatives
	* Drone CI
	* TeamCity(JetBrains)
	* CircleCI(cloud-based servers)

## Installation
	* System
		* Use any Ubuntu Box : for eg. Hashicorp bionic64 (vagrant)
	
	* Java
		* Check for java version : java --version
		* `sudo add-apt-repository ppa:webupd8team/java /`
		* `sudo apt-get update /` 
		* `sudo apt install openjdk-8-jdk`
	
	* Jenkins
		* Add the Jenkins Debian repository: `wget -q -O - https://pkg.jenkins.io/debian/jenkins.io.key | sudo apt-key add -`
		* Adding jenkins repo to system: `sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'`
		* `sudo apt update` and `sudo apt install jenkins`

Checking status of jenkins service : `sudo systemctl status jenkins`

## Adjusting firewall :
	* sudo ufw allow 8080
	* sudo ufw status
	
Go to http://ip_address:8080 
 `cat /var/lib/jenkins/secrets/initialAdminPassword`
 Add admin user details such as username,password,full name,email id.
 