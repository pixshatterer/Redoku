pipeline {
    agent any 

    stages {
        stage('Build Assets') {
          agent any 
          steps {
            nodejs(nodeJSInstallationName: 'Node 11.x', configId: 'latest') {
              sh 'npm config ls'
            }
          }
        }
        stage('Test') {
          agent any
          steps {
              echo 'Testing stuff...'
          }
        }
    }
}