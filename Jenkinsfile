pipeline {
    agent {
        any {
            image 'maven:3.8.1-adoptopenjdk-11'
            args '-v C:/ProgramData/Jenkins/.m2:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                bat 'mvn -B -DskipTests clean package'
            }
        }
    }
}
