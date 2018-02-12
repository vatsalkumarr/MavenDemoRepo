pipeline {
  agent any
  stages {
    stage('clone') {
      steps {
        echo 'in clone'
      }
    }
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'in build'
          }
        }
        stage('perfomace') {
          steps {
            echo 'in performance'
          }
        }
      }
    }
    stage('package') {
      steps {
        echo 'in package'
      }
    }
    stage('test') {
      steps {
        echo 'in test'
      }
    }
    stage('deploy') {
      steps {
        echo 'n deploy'
      }
    }
  }
}