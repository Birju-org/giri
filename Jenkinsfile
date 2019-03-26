node {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/Birju-org/giri.git']]])
            }
        }
        stage('Build') {
            steps {
              sh '/opt/maven/apache-maven-3.6.0/bin/mvn clean package'
            }
        }
        
    }
}

