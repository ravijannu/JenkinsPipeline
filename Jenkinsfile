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
            echo "Testing Ravi Jannu Step${companyname}"
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'Deploy Development Bransh Step'
        input(message: 'WaitForApproval', id: 'Yes')
      }
    }

  }
  environment {
    companyname = 'clickdata'
  }
}