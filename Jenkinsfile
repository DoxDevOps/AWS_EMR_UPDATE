pipeline {
  agent any
  stages {
    stage('Initialising') {
      steps {
        echo 'Initialising to update instance'
      }
    }

    stage('Pulling code from Github') {
      steps {
        echo ' Pulling from github'
        sh '''ssh -o StrictHostKeyChecking=no -i  DevOpsKey.pem ubuntu@ec2-3-21-164-128.us-east-2.compute.amazonaws.com uptime ; cd /var/www/art-poc-setup ;    git pull origin master
; git fetch --tags -f ;    ./update.py ;    sudo docker-compose build

   '''
      }
    }

  }
}