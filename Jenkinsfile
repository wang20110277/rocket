pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'mvn --version'
        sh 'mvn clean'
        sh 'mvn install'
      }
    }

    stage('deploy') {
      steps {
        sh 'mv /Users/lindaw/.jenkins/workspace/DevOps_main/target/rocket-0.0.1-SNAPSHOT.jar /Users/lindaw/Documents/test/'
      }
    }

  }
}