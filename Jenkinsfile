pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
               checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/akshay1996137/JavaWeb.git']]])
            }
        }
        stage('build') {
            steps {
               sh 'mvn test'
            }
        }
    }
}
