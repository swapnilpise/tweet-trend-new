pipeline {
    agent {
        node {
            label 'maven'
        }
    }

environment {
    PATH = "/opt/apache-maven-3.9.9/bin:$PATH"
}
    stages {
        stage("build"){
            steps {
                sh 'mvn clean deploy -Dmaven.surefire.debug -Xms512m -Xmx2048m'
            }
        }
    }
}
