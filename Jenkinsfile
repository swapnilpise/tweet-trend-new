pipeline {
    agent {
        node {
            label 'maven'
        }
    }

    environment {
        MAVEN_OPTS = "-Xms512m -Xmx2048m -XX:MaxPermSize=512m"
    }

    stages {
        stage("Build") {
            steps {
                sh 'mvn clean deploy'
            }
        }
    }
}

