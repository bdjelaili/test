node('docker') {
   docker.image('maven').inside {
      git 'https://github.com/fabric8io/example-camel-cdi'
      sh 'mvn clean install'
   }
}
