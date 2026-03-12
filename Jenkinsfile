pipeline {
agent any


tools {
    jdk 'JDK25'
    maven 'Maven'
}

environment {
    JAVA_HOME = 'C:\\Program Files\\Java\\jdk-25.0.2'
    PATH = "${env.JAVA_HOME}\\bin;${env.PATH}"
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
