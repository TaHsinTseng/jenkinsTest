pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                bat 'python helloworld.py'
                bat 'python add2.py 18 23'
            }
        }
    }
}
