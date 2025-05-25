pipeline {
    agent any

    environment {
        XYZ = 'ITI ITI ITI'
    }

    stages {
        stage("Build Docker image") {
            steps {
                sh "docker build -t yahiazakaria/data-iti1:v${BUILD_NUMBER} ."
            }
        }

        stage("Push Docker image") {
            steps {
                sh "docker push yahiazakaria/data-iti1:v${BUILD_NUMBER}"
            }
        }
    }
}