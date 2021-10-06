pipeline {
    agent any

    stages {
        stage('Vaidation') {
            steps {
                echo 'Validate Project..'
		sh 'mvn validate'
		sh 'mvn compile'
            }
        }
        stage('UnitTest') {
            steps {
                echo 'Testing..'
		sh 'mvn test'
            }
        }
        stage('containerizing') {
            steps {
                echo 'containerizing....'
		sh 'docker run -dt --name raje -p 4550:80 httpd'
            }
        }
    }
}
