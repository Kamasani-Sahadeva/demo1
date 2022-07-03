pipeline {
    agent any

    stages {
        stage(Git checkout from Dev) {
            steps {
                sh "git clone https://github.com/Kamasani-Sahadeva/demo1.git "
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

        
        stage(Deployment to K8s - Dev Env) {
            steps {
                sh "Deployed app to K8s"
            }
        }

    }

}
