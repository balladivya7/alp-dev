pipeline {
    agent any

    stages {
        stage('Clone to Packer Repo') {
            steps {
                git branch: 'main', url: 'https://github.com/piyushmj12/golden_image_packer'
            }
        }
         stage("Running for packer template"){
           steps {
    sh """pwd
    dir('blob/main/aws/templates/aws_ami.pkr.hcl') {
      Packer Build
      pwd"""
    }
    
}
    }
}
