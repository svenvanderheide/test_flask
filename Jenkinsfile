pipeline {
  agent {
    docker {
      image 'python:3.7'
    }

  }
  stages {
    stage('SCM') {
      agent any
      steps {
        sh 'pip install -r requirements.txt'
      }
    }
  }
}