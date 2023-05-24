pipeline {
  agent any
  environment {
    HEROKU_API_KEY = credentials('heroku-api-key')
    IMAGE_NAME = 'darinpope/jenkins-example-react'
    IMAGE_TAG = 'latest'
    APP_NAME = 'jenkins-example-react'
  }
  stages {
    stage('Build') {
      steps {
        sh 'docker build -t $IMAGE_NAME:$IMAGE_TAG .'
      }
    }
  }
}
