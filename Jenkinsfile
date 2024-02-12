pipeline {
  agent any
  
  stages {
    stage('checkout stage') {
      steps {
        sh 'rm -rf grafana_varun'
        sh 'git clone https://github.com/varun-doode/grafana_varun.git'
      }
    }
    stage('running playbook') {
      steps {
        sh 'ansible-playbook -i hosts grafana1.yml'
      }
    }
  }
}
