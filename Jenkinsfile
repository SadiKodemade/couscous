pipeline {
  agent {
    node {
      label 'node_sadi'
    }

  }
  stages {
    stage('') {
      steps {
        git(credentialsId: 'ubuntu', branch: 'main', url: 'https://github.com/SadiKodemade/couscous.git', poll: true)
      }
    }

  }
}