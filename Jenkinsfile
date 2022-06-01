pipeline {
    agent {label 'build_java_11'}

    stages {
        stage ('sourcecode') {
            steps {
                git branch: 'main', url: 'https://github.com/madhu2292/spring-petclinic.git'
            }
        }
        stage('build the code') {
            steps {
               sh 'mvn package'
            }
        }
    }
}
