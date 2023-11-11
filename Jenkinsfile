pipeline {
    agent {
        node{
            label 'maven'
        }
    }

    stages {
        stage('Code Pull') {
            steps {
                git branch: 'main', url: 'https://github.com/pintu121/java-demo-app.git' 
            }
        }
    }
}

