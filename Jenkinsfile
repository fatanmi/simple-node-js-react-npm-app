pipeline {
   
}}
        
       stages {
        stage('Build') { 
            steps {
                node ('non-docker-agent') {

    docker.withServer($DOCKER_SERVER) {

        // Right here we are currently in `non-docker-agent` and Jenkins check if `non-docker-agent` itself runs inside a container
        // It is not, Jenkins says "'non-docker-agent' does not seem to be running inside a container"
        docker.image('$DOCKER_IMAGE').inside {
            sh "hostname"
        }

            }
        }
        }
    }
