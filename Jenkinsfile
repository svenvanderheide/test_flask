pipeline {
  agent {
    docker {
      image 'python:3.7'
    }

  }
  stages {
    stage('SCM') {
      steps {
        sh 'pip3 install -r requirements.txt'
      }
    }
  }
}