pipeline {
  agent any
  
  stages {
    stage('java') {
      agent {
        label 'java'
      }
      
      steps {
        container('java') {
          sh 'java -version'
        }
      }
    }
    
    stage('python') {
      agent {
        label 'python'
      }
      
      steps {
        container('python') {
          sh 'python -V'
        }
      }
    }
    
    stage('go') {
      agent {
        label 'golang'
      }
      
      steps {
        container('golang') {
          sh 'go version'
        }
      }
    }
  }
}
