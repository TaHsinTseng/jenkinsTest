pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                bat 'python helloworld.py'
                bat 'python helloworld.py 1 2'
            }
        }
    }
}
