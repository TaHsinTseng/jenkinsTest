pipeline {
    agent any
    parameters {
        string(name: 'PY_TESTFILE', defaultValue: 'helloworld.py', description: 'Which python script I should run?',)
    }
    stages {
        stage('test') {
            steps {
            	echo 'This is for testing git in sublime.'
                echo "First run standard helloworld."
                bat 'python helloworld.py'
            	bat 'echo "The parameterized python file to run is ${params.PY_TESTFILE}"'
                bat "python ${params.PY_TESTFILE}"
                //python ${params.PY_TESTFILE}
                bat 'python add2.py 18 23'
            }
        }
    }
}
