pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'mvn clean package appassembler:assemble'
      }
    }

    stage('deploy') {
      steps {
        sh 'zip -rqm ./rocket.zip ./rocket'
        sh 'mv ./rocket.zip /Users/lindaw/Documents/'
        sh 'unzip -o /Users/lindaw/Documents/rocket.zip -d /Users/lindaw/Documents/'
      }
    }

  }
}