pipeline {
  agent any
    
  tools {nodejs '7.7.3'}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/QNNAKWUE/Ecommerce-Nodejs.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
         sh '<<Build Command>>'
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'node test'
      }
    }
  }
}