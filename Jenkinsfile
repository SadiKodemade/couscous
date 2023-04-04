pipeline {
  agent {
    node {
      label 'node_sadi'
    }

  }
  stages {
    stage('error') {
      parallel {
        stage('error') {
          steps {
            git(credentialsId: 'ubuntu', branch: 'main', url: 'https://github.com/SadiKodemade/couscous.git', poll: true)
          }
        }

        stage('deploy') {
          steps {
            sh '''rm -r /var/www/couscous/*
git clone https://github.com/SadiKodemade/couscous.git /var/www/couscous 
'''
          }
        }

      }
    }

  }
}