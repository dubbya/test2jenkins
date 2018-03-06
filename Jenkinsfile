pipeline {
  agent any
  options { skipDefaultCheckout() }
  stages {
    stage('Sleep') {
      agent {
        node {
          label 'K2VM'
        }
        
      }
      steps {
        sleep 5
      }
    }
  }
}
