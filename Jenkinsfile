pipeline {
    agent any

    environment {
        REGISTRY = "docker.io/<your-dockerhub-username>"
        APP_NAME = "myapp"
        IMAGE = "${REGISTRY}/${APP_NAME}:${BUILD_NUMBER}"
    }
  
  stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/<your-org>/<your-repo>.git'
            }
        }
  }
}
