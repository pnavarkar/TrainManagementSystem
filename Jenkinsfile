pipeline {
    agent any     

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        
       
        stage('Build') {
            steps {
                echo 'Building..'
                bat "mvn -Dmaven.test.failure.ignore=true clean package"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
   
    }
}
