pipeline {
    agent any
    environment { 
        CC = 'clang'
    }
    stages {
        stage('Example') {
            environment { 
                AN_ACCESS_KEY = credentials('idTest') 
            }
            steps {
                sh 'printenv'
                sh 'echo ${AN_ACCESS_KEY_USR}'
                sh 'echo ${AN_ACCESS_KEY_PSW}'
            }
        }
    }
}
