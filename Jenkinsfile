pipeline {
    agent any
    parameters {
        string(name: 'pyTestFile', defaultValue: 'helloworld.py', description: 'Which python script I should run?')
    }
    stages {
        stage('test') {
            steps {
                python ${params.pyTestFile}
                bat 'python add2.py 18 23'
            }
        }
    }
}
