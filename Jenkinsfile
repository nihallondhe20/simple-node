@Library('shared-libs')__

pipeline {
    agent any
     environment {
        version= '2'
        FILENAME= 'simple-node'
        DOCKER_CREDENTIALS_ID = '7597417b-2339-4ebe-8e53-5c98b09e4fc7'
        DOCKER_REGISTRY_URL = 'https://index.docker.io/v2'
    }

    stages {
        
        stage('install') {
            steps {
                install()
            }
        }
    
        stage('build') {
            steps {
                buld()
            }
        }
        stage('test') {
            steps {
                test()
            }
        }
        stage('deploy') {
           steps{
                script{
                    deploy()
           }
        }
    }
  }
}
