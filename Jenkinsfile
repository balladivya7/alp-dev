pipeline {
    agent any

    stages {
        stage('Clone to Packer Repo') {
            steps {
                git branch: 'main', url: 'https://github.com/piyushmj12/golden_image_packer'
            }
        }
    }
}
