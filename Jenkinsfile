pipeline {
  agent any
  tools {
        maven 'maven'
     }
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
        sh '$mvnHome/bin/mvn package'        
      }
    }
  }
}
