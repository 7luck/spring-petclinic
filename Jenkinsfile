pipeline {
  agent any

  stages {
    stage ("Build") {
        steps {
            sh "mvn -version"
            sh "./mvnw package"
        }
    }
  }

  post {
    always {
      cleanWs()
    }
  }
}
