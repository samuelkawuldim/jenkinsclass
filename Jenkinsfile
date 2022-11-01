  pipeline {
    agent none
    tools {
        maven 'local maven' 
    }
    stage('Checkout') {
      steps {
        git url: 'https://github.com/samuelkawuldim/jenkinsclass.git',
          credentialsId: 'TT',
            branch 'main'
