pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo '"to Build"'
      }
    }

    stage('test') {
      steps {
        echo 'to test'
      }
    }

    stage('stage') {
      parallel {
        stage('stage') {
          steps {
            echo 'to stage'
          }
        }

        stage('deploy') {
          steps {
            echo 'to deploy'
          }
        }

        stage('operate') {
          steps {
            echo 'to operate'
          }
        }

      }
    }

  }
}