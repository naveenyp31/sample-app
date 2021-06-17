pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
                git credentialsId: 'Git_cred', 
                url: 'https://github.com/naveenyp31/sample-app.git'
            }              
        }
        stage('Build') {
            steps {
                sh "mvn clean install"
            }       
        }     
    }
}