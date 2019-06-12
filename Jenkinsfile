pipeline {
  agent any
  tools {
        maven 'maven'
     }
  stages {
    stage('Build') {
      steps {
        def mvnHome = tool 'maven'
        sh '$mvnHome/bin/mvn package'        
      }
    }
  }
}
