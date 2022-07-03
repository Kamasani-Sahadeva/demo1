pipeline {
    agent any

    stages {
        stage(Git checkout from main) {
            steps {
                sh "git clone "
            }
        }

        
        stage(Git checkout-Dev ) {
            steps {
                sh "echo cloned git repo "
            }
        }

        
        stage(Build code) {
            steps {
                sh "echo build code & Test completed "
            }
        }

         
        stage(Sonarqube) {
            steps {
                sh "echo code scanning and security scanning completed "
            }
        }

         
        stage(Build docker image) {
            steps {
                sh "echo building docker image "
            }
        }

        
        stage(Push image to docker hub) {
            steps {
                sh "echo pushed image to dockerhub"
            }
        }

        
        stage(Image scanning) {
            steps {
                sh "echo image scanning"
            }
        }

        
        stage(Deployment to K8s - main Env) {
            steps {
                sh "Deployed app to K8s"
            }
        }

    }

}
