pipeline {
  agent {
    docker {
      image 'litemall-api'
      args '-v /root/.m2:/root/.m2'
    }

  }
  stages {
    stage('complie') {
      agent {
        node {
          label 'web.an7yun'
        }

      }
      steps {
        sh 'mvn clean install'
      }
    }
  }
}
