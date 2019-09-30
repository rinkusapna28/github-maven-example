pipeline {
    agent {label 'slave-node'}
    stages {
        stage('clone git repo') {
            steps {
                git 'https://github.com/kevinsawicki/github-maven-example'
            }
        }
		stage('Compile') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
