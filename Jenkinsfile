pipeline {
    agent any

    stages {
        stage('Git clone') {
            steps {
                git branch: 'main', url: 'https://github.com/manjushachalla/spring-petclinic.git'
            }
        }
        stage('Generate build') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
