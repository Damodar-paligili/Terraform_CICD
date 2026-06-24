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
                sh 'cd DAY-1-BASICS'
                sh 'terraform init'
            }
        }
    stage('Debug') {
            steps {
        sh '''
        pwd
        ls -la
        find . -name "*.tf"
        '''
        }
        }
   stage('plan') {
            steps {
                
                sh 'terraform plan'
            }
        }
    }
}
