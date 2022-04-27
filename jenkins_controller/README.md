docker build -t my_jenkins:latest .

docker run --name my_jenkins --rm --detach -p 8081:8080 -p 50001:50000 -v C:\Users\grzel\PandaAcademy\my-work\artifactory\jenkins_controller\casc.yml:/usr/share/jenkins/ref/casc.yml my_jenkins