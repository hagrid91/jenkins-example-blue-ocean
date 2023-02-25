pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date
cal 2023'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test step'
          }
        }

        stage('test parallel') {
          steps {
            echo 'test jar'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy jar'
      }
    }

  }
}