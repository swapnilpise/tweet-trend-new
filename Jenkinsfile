pipeline {
    agent {
        node {
            label 'maven'
        }
    }

    environment {
        PATH = "/opt/apache-maven-3.9.9/bin:$PATH" // Adjust this path as necessary
    }

    stages {
        stage("Build") {
            steps {
                sh 'mvn clean deploy'
            }
        }
    }
}

