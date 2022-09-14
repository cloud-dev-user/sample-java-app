pipeline {
  agent {
    node {
      label 'node_1.4'
    }

  }
  stages {
    stage('build CI ') {
      steps {
        sh 'mvn clean package'
      }
    }

    stage('invoke learnwell class ') {
      steps {
        sh 'java -cp target/devops-1.0-SNAPSHOT.jar learnwell.app.App '
      }
    }

  }
}