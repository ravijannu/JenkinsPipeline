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
            echo 'Testing Step'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        sh '''#!/bin/ksh
# Tested with ksh version JM 93t+ 2010-03-05
for i in {1..100}
do
 # your-unix-command-here
 echo $i
done'''
      }
    }

  }
}