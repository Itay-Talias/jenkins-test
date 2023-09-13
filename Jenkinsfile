pipeline {
    agent any
    stages {
        stage('install dependencies') {
            steps {
                echo 'hii'
            }
        } stage('Test') {
            steps {
                echo 'Testing....' sh 'python3 -m pytest test_add.py'
            }
          }
        }
    }