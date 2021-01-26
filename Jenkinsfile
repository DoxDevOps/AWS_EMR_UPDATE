pipeline {
  agent any
  stages {
    stage('Initialising') {
      steps {
        echo 'Initialing to update instance'
      }
    }

    stage('Pulling code from Github') {
      steps {
        echo 'Stsrting to pull from github'
        sh 'git clone https://github.com/HISMalawi/BHT-EMR-API.git'
      }
    }

  }
}