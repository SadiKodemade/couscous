pipeline {
  agent {
    node {
      label 'node_sadi'
    }

  }
  stages {
    stage('deploy') {
      steps {
        sh '''rm -r /var/www/couscous/*
git clone https://github.com/SadiKodemade/couscous.git /var/www/couscous 
'''
      }
    }

  }
}