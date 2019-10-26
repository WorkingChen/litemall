pipeline {
  agent {
    docker {
      image 'litemall-api'
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