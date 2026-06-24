pipeline {
    agent any

    stages {
        stage('clone') {
            steps {
              git branch: 'main', url: 'https://github.com/Damodar-paligili/terraform-9am.git'
            }
        }
        stage('change directory')  {
            steps {
                sh 'cd DAY-1-BASICS'
            }
        }

        stage('init') {
            steps {
                sh 'terraform init'
            }
        }
         stage('plan') {
            steps {
                sh 'terraform plan'
            }
        }
    }
}
