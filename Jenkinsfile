pipeline {
    agent any
    environment {
        AWS_ACCOUNT_ID="011138670495"
        AWS_DEFAULT_REGION="us-east-2"     
    }
    stages {
        
        stage('provision eks-cluster') {
           environment {
             AWS_ACCESS_KEY_ID = credentials('aws_access_key_id')
             AWS_SECRET_ACCESS_KEY = credentials('aws_secret_access_key')
           }
           steps {
              script {
                  sh "terraform destroy --auto-approve"
//                   sh "terraform init"
//                   sh "validate"
//                   sh "terraform plan"
//                   sh " terraform apply --auto-approve"
            }
        }
               
     }
    }
    
}
