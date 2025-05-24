pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
ls
date'''
      }
    }

    stage('Testing') {
      parallel {
        stage('Testing') {
          steps {
            echo 'Testing the Build'
          }
        }

        stage('Testing Parallel') {
          steps {
            echo 'Testing Service Build'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying the Service.......'
      }
    }

  }
}