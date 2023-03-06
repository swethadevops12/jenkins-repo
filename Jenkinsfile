pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'i want to build'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'i want to test'
          }
        }

        stage('deploy') {
          steps {
            echo 'i want to deploy'
          }
        }

      }
    }

  }
}