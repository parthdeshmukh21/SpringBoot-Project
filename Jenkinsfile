pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/parthdeshmukh21/SpringBoot-Project.git'
            }
        }

        stage('Build with Maven') {
            steps {
                withMaven(maven: 'maven') {
                    sh 'mvn clean package'
                }
            }
        }
    }
}

