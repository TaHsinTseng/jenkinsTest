pipeline {
    agent any
    parameters {
        string(name: 'pyTestFile', defaultValue: 'helloworld', description: 'Which python script I should run?')
    }
    stages {
        stage('test') {
            steps {
                bat 'python ${param.pyTestFile}.py'
                bat 'python add2.py 18 23'
            }
        }
    }
}
