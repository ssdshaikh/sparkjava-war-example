pipeline {
  agent any
  stages {
    stage('initialize') {
      steps {
        sh '''
        echo "PATH = ${PATH}"
        echo "M2_HOME = ${M2_HOME}"
        '''
      }
    }
    stage('Build') {
      steps {
        sh 'mvn sonar:sonar install'
      }
    }
  }
  tools {
    maven 'maven'
  }
}
