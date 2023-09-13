pipeline {
    agent any
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