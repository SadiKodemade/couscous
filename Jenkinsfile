pipeline {
  agent {
    node {
      label 'node_sadi'
    }

  }
  stages {
    stage('deploy') {
      steps {
        sh '''sudo rm -rf /var/www/couscous
sudo mkdir /var/www/couscous
sudo git clone https://github.com/SadiKodemade/couscous.git /var/www/couscous 
'''
      }
    }

  }
}