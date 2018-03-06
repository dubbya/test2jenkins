pipeline {
  agent any
  stages {
    stage('Sleep') {
      agent {
        node {
          label 'K2VM'
        }
        
      }
      steps {
        sleep 5
        powershell(script: 'c:\\test.ps1', returnStatus: true, returnStdout: true)
      }
    }
  }
  options {
    skipDefaultCheckout()
  }
}