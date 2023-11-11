pipeline {
    agent {
        node{
            label 'maven'
        }
    }
enveironment {
    PATH = "/opt/apache-maven-3.9.5/bin:$PATH"
}
    stages {
        stage('Code Pull') {
            steps {
                git branch: 'main', url: 'https://github.com/pintu121/java-demo-app.git' 
            }
        }
    }
    stages {
        stage('Build code') {
            steps {
                sh 'mvn clean deploy'
            }
        }
    }
}

