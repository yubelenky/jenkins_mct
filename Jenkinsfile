pipeline {
  agent {
      docker {
          image 'hashicorp/terraform:latest'
          label 'TF-AGENT'
          args  '--entrypoint="" -u root -v /opt/jenkins/.aws:/root/.aws'
      }
  }  
  environment {
    TF_WORKSPACE = 'dev' //Sets the Terraform Workspace
    TF_IN_AUTOMATION = 'true'
  }
  stages {
    stage('Terraform Init') {
      steps {
        sh 'mkdir /home/ec2-user/newjenkins'
      }
    }
  }
}