pipeline {
  agent {
    docker {
      image 'python:3.7'
    }

  }
  stages {
    stage('SCM') {
      steps {
        sh 'pip install -r requirements.txt'
      }
    }
  }
}