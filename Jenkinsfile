pipeline {
    agent any

    stages {
        stage('starting docker') {
            steps {
                echo 'start docker....'
		sh 'sudo systemctl start docker'
            }
	stage('containerizing') {	
            steps {
                echo 'containerizing....'
		sh 'docker run -dt --name raej -p 3333:80 httpd'
            }
        }
    }
  }
}
