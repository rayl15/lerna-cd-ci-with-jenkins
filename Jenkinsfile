pipeline {
  
  agent { 
    docker { 
      image 'node:10' 
    } 
  }

  stages {
    stage('Build') {
      steps {
        echo 'Building...'
        sh 'npm install'
      }
    }
    stage('Test') {
      steps {
        echo 'Testing...'
        sh 'npm test'
      }
    }
  }
}