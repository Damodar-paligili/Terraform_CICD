pipeline {
    agent any

    stages {
        stage('clone') {
            steps {
              git branch: 'main', url: 'https://github.com/Damodar-paligili/terraform-9am.git'
            }
        }
        

     stage('init') {
            steps {
                dir('DAY-1-BASICS'){
                sh 'terraform init'
            }
            }
        }
   
   stage('plan') {
            steps {
                
                sh 'terraform plan'
            }
        }
    }
}
