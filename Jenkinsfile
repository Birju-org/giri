node {
        stage('Checkout') {
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/Birju-org/giri.git']]])
        }
        stage('Build') {
                sh '${M2_HOME}/bin/mvn clean package'
            }
}

