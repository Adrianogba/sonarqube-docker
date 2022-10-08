# SonarQube Community on Docker
With this, you will be able to easily run the latest version of SonarQube on a Docker Container.
This docker-compose will also create and automatically configure a instance of PostgreSQL 12, which is a requirement for SonarQube to work.

## Requirements
### Docker
Download it here: https://www.docker.com/products/docker-desktop/
*  For Windows users: I personally recommend you use the Windows Subsystem for Linux (WSL) 2 configuration, for better performance. Here is what it is and how to do it:  https://docs.docker.com/desktop/windows/wsl/
### Node.js
Download it here: https://nodejs.org/en/download/
### Sonnar Scanner
Command to install: `npm install -g sonarqube-scanner`

## How to set up and run
Once you have the Docker installed and configured, inside the folder that have the `docker-compose.yml` folder, run:
<br>
`docker-compose up -d`
<br>

## Configure SonarQube
* Open the default page (default credentials and url just below)
* Click in Create Create Project and select Manually
* Once you define the name and key, it will show you the token that the project will use to be scanned.

## How to scan your code
Create/Copy the `sonar-project.properties` file inside the project that you want to scan, changing the following properties:
* `sonar.projectKey` (defined by you when configuring the project on the SonarQube page)
* `sonar.login` (token of the project, defined while configuring the project)
* `sonar.projectName` (name of the project, just to help you identify it on the SonarQube page)

## Scanning the code:
Just run: 
<br>
`sonar-scanner`
<br>
Wait the scan, and when it finishes you will be able to see the results on the SonarQube page.

## Configuration
Default URL: http://localhost:9000/
<br>
Default credentials:
<br>
Login: `admin`
<br>
Password: `admin`

## Documentation
Full documentation: https://docs.sonarqube.org/latest/
<br>
Quick Guide: https://docs.sonarqube.org/latest/setup/get-started-2-minutes/
