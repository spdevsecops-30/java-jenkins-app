pipeline {
    agent any
    options { skipDefaultCheckout(true) }
    stages {
        stage('Checkout') {
            steps { checkout scm }
        }
        stage('Compile') {
            steps { sh 'javac Hello.java' }
        }
        stage('Run') {
            steps { sh 'java Hello' }
        }
    }
}
