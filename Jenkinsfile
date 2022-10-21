pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
               checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/akshay1996137/ecomm.git']]])
            }
        }
    }
}
