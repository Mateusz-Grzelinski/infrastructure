# run

docker build -t jenkins_agent:latest .

docker run -d --rm --name jenkins_agent -p 222:22 -e "JENKINS_AGENT_SSH_PUBKEY=ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCaJxXl+C4GsmIcrsXQ+mqS/t9SNsFrtj5LffdnNr8+9a40UUHDX1mKe26U8oSarCciLYEtXWsWtl1VmQS6JAdVI5vZKS2J0Nt6oe+AH9y2PhL6wtqUsel2aJHUk8w13Dfkt+w6tZBQxCuzBDvWRt6hsprVuJvWoICMZanVOoXb+BfJx9133mG/uviF/rgtEqn5CqTbHWN1cUs+jei0GOlfyQr/GR7P5cP6baxe5yxCebohlgbYvDrwUT2ZBSlJHIaqbrbeBF/yigCcWCA9z46PubKc/qIcDY5qeFuldy0mqEdpMILDLjcrtidnp4wvRa8cxZl4w9fNYGwK8C56/b9n" 
-v /var/run/docker.sock:/var/docker.sock 
jenkins_agent:latest 


## inne demo

docker run -d --name sonarqube -p 9000:9000 sonarqube:9.2.4-community
