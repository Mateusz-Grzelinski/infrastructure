docker build -t my_jenkins:latest .

docker run --name my_jenkins --rm --detach -p 8081:8080 -p 50001:50000 -v C:\Users\grzel\PandaAcademy\my-work\artifactory\jenkins_controller\casc.yml:/usr/share/jenkins/ref/casc.yml my_jenkins


docker run -d --name sonarqube -p 9000:9000 sonarqube:9.2.4-community
docker run --name artifactory -d -p 8082:8081 -p 8083:8082 -v C:\Users\grzel\PandaAcademy\my-work\artifactory:/artifactory_extra_conf artifactory

