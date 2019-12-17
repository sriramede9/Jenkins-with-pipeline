pipeline {
    agent any
    stages {
        stage('---clean---') {
            steps {
                bat "git clone https://github.com/pknowledge/my-app.git"
                bat "mvn clean -f my-app"
            }
        }
        stage('--test--') {
            steps {
                bat "mvn test -f my-app"
            }
        }
        stage('--package--') {
            steps {
                bat "mvn package -f my-app"
            }
        }
    }
}