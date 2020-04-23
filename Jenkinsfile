pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            //args '-p 3000:3000' 
            args '-H tcp://0.0.0.0:2375'
        }}
        
       stages {
        stage('Build') { 
            steps {
                
                //sh 'npm install' 
                sh "docker ps"
            }
        }
        }
    }
