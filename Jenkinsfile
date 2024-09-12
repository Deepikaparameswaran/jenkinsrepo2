pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build executed successfully'
      }
    }

    stage('Dev') {
      parallel {
        stage('Dev') {
          steps {
            echo 'Dev executed'
          }
        }

        stage('QA') {
          steps {
            echo 'QA executed'
          }
        }

      }
    }

    stage('Prod') {
      steps {
        echo 'Prod executed successfully'
      }
    }

  }
}