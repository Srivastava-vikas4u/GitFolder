pipeline {
    agent any

    stages {
        stage('Build Hello') {
            steps {
                echo 'Build World'
            }
        }
        stage('Deploy Hello') {
            steps {
                echo 'Deploy World'
            }
        }
        stage('Test Hello') {
            steps {
                echo 'Test World'
            }
        }
    }
    post 
    {
        failure
        {
            emailext body: 'ProjectTest fail', subject: 'ProjectTest fail', to: 'srivastava.vikas4u@gmail.com'
        }
    }
}
