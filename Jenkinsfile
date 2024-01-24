pipeline {
    agent {
        node {
            label 'maven-build'
        }
    }
    environment {
        PATH = "/opt/apache-maven-3.9.6/bin:$PATH"
    }
    stages {
        stage("Build") {
            steps {
                sh 'echo Webhooks is working'
                sh 'mvn clean deploy'
            }
        }
    }
}
