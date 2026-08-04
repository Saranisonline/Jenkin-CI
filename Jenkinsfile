pipeline {
    agent any

    tools {
        maven 'Maven'
    }

    stages {
        stage('Compile') {
            steps {
                dir('DemoProject') {
                    bat 'mvn compile'
                }
            }
        }

        stage('Test') {
            steps {
                dir('DemoProject') {
                    bat 'mvn test'
                }
            }
        }

        stage('Package') {
            steps {
                dir('DemoProject') {
                    bat 'mvn package'
                }
            }
        }
    }
}
