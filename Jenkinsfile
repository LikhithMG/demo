pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/LikhithMG/demo.git'
            }
        }
         stage('Run Python Script') {
            steps {
                sh 'python3 --version'
                sh 'python3 bin.py'
            }


        stage('Run Script') {
            steps {
                sh 'chmod +x script.sh'
                sh './script.sh'
            }
        }
       
    }
}
