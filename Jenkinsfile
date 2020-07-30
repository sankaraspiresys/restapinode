pipeline {  
    environment {
        registry = "sankardockerdev / samplenodeapp"
        registryCredential = 'sankardockerdev'
    }  
    agent any  
    stages {
        stage('Building image') {
        steps{
            script {
            docker.build registry + ":$BUILD_NUMBER"
            }
        }
        }
  }
}