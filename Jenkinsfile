pipeline {
  agent {
    docker {
      image 'python:3.7'
    }

  }
  stages {
    stage('SCM') {
      agent any
      environment {
        FLASK_APP = 'index.py'
      }
      steps {
        sh '''echo $(ls)
echo $(cat requirements.txt)
echo $(pwd)
pip install -r requirements.txt
flask run'''
      }
    }
  }
  environment {
    p = '5000:5000'
  }
}