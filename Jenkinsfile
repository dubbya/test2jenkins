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
        def msg = powershell(returnStdout: true, script: 'Write-Output "PowerShell is mighty!"')
        println msg
      }
    }
  }
  options {
    skipDefaultCheckout()
  }
}
