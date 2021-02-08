pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'mvn clean'
        sh 'mvn install'
      }
    }

    stage('deploy') {
      steps {
        sh 'mv /Users/lindaw/.jenkins/workspace/rocket_main/target/rocket-0.0.1-SNAPSHOT.jar /Users/lindaw/Documents/test/'
      }
    }

  }
}