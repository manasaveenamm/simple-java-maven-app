pipeline {
agent any


tools {
    jdk 'JDK25'
    maven 'Maven'
}

stages {
    stage('Checkout') {
        steps {
            git 'https://github.com/manasaveenamm/simple-java-maven-app.git'
        }
    }

    stage('Build') {
        steps {
            bat 'mvn clean package'
        }
    }
}


}
