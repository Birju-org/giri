node {
        stage('Checkout') {
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/Birju-org/giri.git']]])
        }
        stage('Build') {
              sh '/opt/maven/apache-maven-3.6.0/bin/mvn clean package'
            }
}

