node {
        stage("Main build") {

            checkout scm

            docker.image('ubuntu:16.04').inside {

              stage("Install JDK 8 (latest edition)") {
                sh "sudo apt-get install openjdk-8-jdk"
              }
                    
           }

        }

}
