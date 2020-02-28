## Jenkins Installation
We need to install jenkins container first using docker. Get the latest version of jenkins.
Command:
`docker run -d -u root --name jenkins \
    -p 9090:8080 -p 50000:50000 \
    -v /root/jenkins_2112:/var/jenkins_home \
    jenkins/jenkins
`{{execute}}
After you run the command you can visit vi dashboard tab and change port to 9090.

You need password? let's check it `docker exec -it jenkins cat /var/jenkins_home/secrets
/initialAdminPassword`{{execute}}

For jenkins installation you just select recomendation plugins. After that skip the password setup and others.