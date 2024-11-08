pipeline {
    agent {
        node {
            label 'maven'
        }
    }

environment {
    PATH = "/usr/share/maven-3.8.7/bin:$PATH"
}
    stages {
        stage("build"){
            steps {
                sh 'mvn clean deploy'
            }
        }
    }
}