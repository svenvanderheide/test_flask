pipeline {
  agent {
    docker {
      image 'python:3.7'
    }

  }
  stages {
    stage('SCM') {
      agent {
        docker {
          image 'python:3.7'
        }

      }
      steps {
        sh 'pip install -r requirements.txt'
      }
    }
  }
}