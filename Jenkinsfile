pipeline {
    agent any 

    stages {
        stage('Build Assets') {
          agent any 
          steps {
            nodejs(nodeJSInstallationName: 'Node 6.x', configId: '<config-file-provider-id>') {
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