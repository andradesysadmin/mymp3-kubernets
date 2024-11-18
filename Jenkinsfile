pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    git 'https://github.com/andradesysadmin/mymp3-kubernets.git'
                }
            }
        }

        stage('Apply') {
            steps {
                script {
                    sh 'kubectl apply -f manifests/'
                }
            }
        }
    }
}
