docker.image('maven').inside {

    stage("Install Bundler") {
      sh "git 'https://github.com/fabric8io/example-camel-cdi'"
    }

    stage("Use Bundler to install dependencies") {
      sh "mvn clean install"
    }
}
