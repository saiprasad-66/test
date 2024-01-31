pipeline {
  agent any
  stages {
    stage('Dev') {
      steps {
        echo 'this is dev stage'
      }
    }

    stage('Build') {
      steps {
        echo 'this is build stage'
      }
    }

    stage('test') {
      steps {
        echo 'this is test stage'
      }
    }

    stage('UAT') {
      parallel {
        stage('UAT') {
          steps {
            echo 'this is UAT stage'
          }
        }

        stage('Deploye') {
          steps {
            echo 'this is deploy stage'
          }
        }

        stage('Operate') {
          steps {
            echo 'this is operate stage'
          }
        }

      }
    }

  }
}