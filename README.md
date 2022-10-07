# SonarQube Community on Docker
With this, you will be able to easily run the latest version of SonarQube on a Docker Container.
This docker-compose will also create and automatically configure a instance of PostgreSQL 12, which is a requirement for SonarQube to work.

## Requirements
You will need the Docker configured on your machine to proceed. Download it here: https://www.docker.com/products/docker-desktop/
*  For Windows users: I personally recommend you use the Windows Subsystem for Linux (WSL) 2 configuration, for better performance. Here is what it is and how to do it:  https://docs.docker.com/desktop/windows/wsl/


## How to set up and run
`docker-compose up -d`
<br>

## How to use
Default URL: http://localhost:9000/
<br>
Default credentials:
<br>
Login: `admin`
<br>
Password: `admin`

## How to use SonarQube
Documentation: https://docs.sonarqube.org/latest/
<br>
Quick Guide: https://docs.sonarqube.org/latest/setup/get-started-2-minutes/
