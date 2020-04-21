pipeline {
    agent {
        docker {
            image 'node:alpine' 
            args '-p 3000:3000' 
        }}
        
       stages {
        stage('Build') { 
            steps {
                // sh "sudo npm install --unsafe-perm=true --allow-root"
                sh 'npm install' 
            }
        }
        }
    }
