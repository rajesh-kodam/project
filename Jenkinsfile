pipeline {
    agent any

    stages {
        stage('starting docker') {
            steps {
                echo 'start docker....'
		sh 'sudo systemctl start docker'
            }
            steps {
                echo 'containerizing....'
		sh 'docker run -dt --name rajj -p 4444:80 httpd'
            }
        }
    }
}
