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
        sh '''echo $(ls)
echo $(cat requirements.txt)
echo $(pwd)
pip install -r requirements.txt'''
      }
    }
  }
}