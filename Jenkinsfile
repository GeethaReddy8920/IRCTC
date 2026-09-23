pipeline {
   agent any
   environment {
      PATH = " /opt/maven/bin:$PATH"
   } 

   stages {
     state('git clone') {
       steps {
         git url: 'https://github.com/GeethaReddy8920/IRCTC.git', branch:'main'
       } 
    }      
   stage('build') {
     steps {
      sh 'mvn clean package'
        }
      }
    }
  }


