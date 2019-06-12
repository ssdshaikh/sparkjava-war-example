pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn package'
        tool(name: 'maven', type: 'maven')
      }
    }
  }
}