pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'Build Test'
          }
        }

        stage('test') {
          steps {
            echo '"Testing Step${companyname}"'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'Deploy Step'
      }
    }

  }
  environment {
    companyname = 'clickdata'
  }
}