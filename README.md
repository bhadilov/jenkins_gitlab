# jenkins_gitlab
This is for setting up Jenkins and Gitlab using a docker-compose file

1. Jenkins
2. Gitlab
3. Nexus Repo


Jenkins Setup

Gitlab Setup
1. All the configuration happens in the gitlab.rb file. Unicorn and nginx will attempt to use the 8080 port which is also setup by default to be used by the http server. These ports will need to be modified in that gitlab.rb file
2. For audit and tracebility purposes, the CI file will be part of the repo and all changes can be tracked.


Jenkins
1. No extra setup was done and still uses the original image from DockerHub



How to Run.

Prerequsites: 
* Make sure docker is installed in the host and updated to the latest version.
* Make sure no other app is using port 8080 and Jenkins will be using it



1. Clone the repo to your machine
2. cd into the working directly and ls to make sure the docker-compose file is present
3. Run docker-compose up -d; this should run the containers in detached mode and setup both Jenkins and Gitlab

Author: Kuhle Nkondeshe
Original date: 16-April-2019