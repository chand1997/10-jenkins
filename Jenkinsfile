pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('kuyya') {
            steps {
                echo 'Hello kuyya'
            }
        }

        stage('bruh') {
            steps {
                echo 'Hello bruh'
                error 'Testing failure in post'
            }
        }
    }

      post { 
        always { 
            echo 'I will always say Hello again!'
        }
        success {
            echo 'Success message!!!'
        }
        failure {
            echo 'Failed!!'
        }
    }
}