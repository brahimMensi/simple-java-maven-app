pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Demo Application'
        sh 'sh `mvn  compile`'
      }
    }

    stage('Test') {
      steps {
        sh 'sh `mvn test`'
      }
    }

    stage('Deliver') {
      steps {
        sh 'sh `mvn --version`'
      }
    }

  }
}