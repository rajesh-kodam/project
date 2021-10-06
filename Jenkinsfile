pipeline {
    agent any

    stages {
        stage('containerizing') {
            steps {
                echo 'containerizing....'
		sh 'docker run -dt --name raj -p 5555:80 httpd'
            }
        }
    }
}
