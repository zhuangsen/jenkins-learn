pipeline {
  stage('Initialize'){
      def dockerHome = tool 'myDocker'
      env.PATH = "${dockerHome}/bin:${env.PATH}"
  }
  
  agent {
    docker {
      image 'maven:3.9.4'
    }

  }
  stages {
    stage('Stage 1') {
      parallel {
        stage('Stage 1') {
          steps {
            echo 'Hello world!'
          }
        }

        stage('Stage 2') {
          steps {
            echo 'hello stage2'
          }
        }

        stage('Stage 3') {
          steps {
            sleep 5
          }
        }

      }
    }

  }
}
