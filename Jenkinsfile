pipeline {
    agent { docker { image 'python_with_pytest:latest' } }
    stages {
        stage('Test') {
            steps {
                parallel(
                    a: {
                        sh "python -m pytest test_add1.py"
                    },
                      b: {
                        sh "python -m pytest test_add2.py"
                      }
                )
            }
          }
    }
}
