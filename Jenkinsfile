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
        sh '''ssh -tt  ubuntu@ec2-3-21-164-128.us-east-2.compute.amazonaws.com ; cd /var/www/art-poc-setup ;    git pull origin master
; git fetch --tags -f ;    ./update.py ;    sudo docker-compose build

   '''
      }
    }

  }
}