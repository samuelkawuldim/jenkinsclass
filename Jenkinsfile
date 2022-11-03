 pipeline {
    agent any
    tools {
        maven "local maven"
    }
    environment {

    PATH = "C:\\WINDOWS\\SYSTEM32"

}

    stages {
        stage('Checkout') {
            steps {
                // Get some code from a GitHub repository
                git url: 'https://github.com/samuelkawuldim/jenkinsclass.git', 
                    branch: 'main',
                    credentialsId: '56fb3b0a-9bf9-4ea5-9187-61a35c3ea15a'
            }
        }
        stage('Build') {
            steps {
                bat 'mvn -B -DskipTests clean package'
            }
        }
    }
}
   
