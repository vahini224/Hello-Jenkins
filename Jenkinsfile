pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/vahini224/Hello-Jenkins/edit/main/Jenkinsfile.git'
            }
        }
    }

    post {
        failure {
            echo 'This block is failure'
        }

        success {
            echo 'This block is success'
        }
    }
}
