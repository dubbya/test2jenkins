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
        powershell(script: '\'Write-Output "PowerShell is mighty!"\'', returnStdout: true)
      }
    }
  }
  options {
    skipDefaultCheckout()
  }
}
