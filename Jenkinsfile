pipeline {
    agent any

    stages {
        stage('gitcheckout') {
            steps {
                git branch: 'main', credentialsId: 'd12662da-ddb5-4fc0-8366-5032015ac591', url: 'https://github.com/aa-sri/DockerFile'
                git branch: 'main', url: 'https://github.com/aa-sri/DockerFile.git'
                sh 'sudo docker build . -t snowflake1:latest'
                sh 'sudo docker run snowflake1'
            }
        }
    }
}
