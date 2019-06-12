pipeline {
  agent any
  tools {
        maven 'maven'
     }
  stages {
    stages {
      stage ("initialize") {
        steps {
          sh '''
          echo "PATH = ${PATH}"
          echo "M2_HOME = ${M2_HOME}"
          '''
          }
        }
    stage('Build') {
      steps {
        def mvnHome = tool 'maven'
        sh '$mvnHome/bin/mvn package'        
      }
    }
  }
}
