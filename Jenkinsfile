pipeline {
    agent any

    environment {
        PATH = "/opt/maven/bin:${env.PATH}"
    }

    stages {
        stage('git clone') {
            steps {
                git url: 'https://github.com/GeethaReddy8920/IRCTC.git', branch: 'main'
            }
        }

        stage('build') {
            steps {
                sh 'which mvn'
                sh 'mvn -version'
                sh 'mvn clean package'
            }
        }
    }
}


