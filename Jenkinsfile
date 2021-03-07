pipeline {
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