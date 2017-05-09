docker.image('maven').inside {

    stage("Install Bundler") {
      git "https://github.com/fabric8io/example-camel-cdi"
    }

    stage("Use Bundler to install dependencies") {
      sh "mvn clean install"
    }
}
