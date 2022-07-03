pipeline {
    agent any

    stages {
        stage("Git checkout") {
            steps {
                git branch: 'main', url: 'https://github.com/Kamasani-Sahadeva/demo1.git'
            }
        }
        
        stage("Build code") {
            steps {
                sh "echo build code"
            }
        }

         
        stage("Sonarqube") {
            steps {
                sh "echo code scanning and security scanning completed "
            }
        }

         
        stage("Build docker image") {
            steps {
                sh "echo building docker image "
            }
        }

        
        stage("Push image to docker hub") {
            steps {
                sh "echo pushed image to dockerhub"
            }
        }

        
        stage("Image scanning") {
            steps {
                sh "echo image scanning"
            }
        }

        
        stage("Deployment to K8s - Prod Env") {
            steps {
                sh "echo Deployed app to K8s"
            }
        }

    }

}
