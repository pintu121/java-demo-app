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
        stage('Build code') {
            steps {
                sh 'mvn clean deploy'
            }
        }
    }
}

