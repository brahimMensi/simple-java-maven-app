pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'pwd'
        echo 'Build Demo Application'
        sh 'sh \'mvn compile\''
      }
    }

    stage('Test') {
      steps {
        sh 'sh `mvn test`'
      }
    }

    stage('Deliver') {
      steps {
        sh 'sh `./jenkins/scripts/deliver.sh`'
      }
    }

  }
}