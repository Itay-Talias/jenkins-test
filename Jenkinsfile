pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                parallel(
                    a: {
                        echo "python -m pytest test_add1.py"
                    },
                      b: {
                        echo "python -m pytest test_add2.py"
                      }
                )
            }
          }
    }
}