 pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                script {
                    checkout([$class: 'GitSCM', branches: [[name: '*/main']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'git credential', url: 'https://github.com/Sanjairamrt/first-maven.git']]])
                }
            }
        }

        stage('Hello World') {
            steps {
                echo 'Hello, World!'
                // Your additional build steps go here
            }
        }
    }
}
