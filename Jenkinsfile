pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/sinchanahegde-15/MyMavenToGradle.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Run') {
            steps {
                sh 'java -jar target/*.jar'
            }
        }
    }
}
