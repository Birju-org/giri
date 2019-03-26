pipeline {
    stages {
        stage('Checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/Birju-org/giri.git']]])
            }
        }
        stage('Build') {
            steps {
                mvn clean install
            }
        }
        
    }
}

