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
        powershell(script: 'c:\\test55.ps1', returnStatus: true, returnStdout: true)
      }
    }
  }
  options {
    skipDefaultCheckout()
  }
}