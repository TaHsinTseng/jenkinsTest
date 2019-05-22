pipeline {
    agent any
    parameters {
        string(name: 'PY_TESTFILE', defaultValue: 'helloworld.py', description: 'Which python script I should run?',)
    }
    stages {
        stage('test') {
            steps {
            	echo 'This is for testing git in sublime.'
            	echo "The python file to run is ${params.PY_TESTFILE}"
                python helloworld.py
                //python ${params.PY_TESTFILE}
                bat 'python add2.py 18 23'
            }
        }
    }
}
