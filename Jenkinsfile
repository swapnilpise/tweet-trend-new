pipeline {
    agent {
        node {
            label 'maven'
        }
    }

    environment {
        MAVEN_OPTS = "-Xmx2048m -Xms512m"
    }

    stages {
        stage("Build") {
            steps {
                sh 'mvn clean deploy -DargLine="-Xmx2048m"'
            }
        }
    }
}

