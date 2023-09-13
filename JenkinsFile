pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                sh 'python -m unittest discover -s path/to/tests -p "test_*.py"'
            }
        }
    }
}