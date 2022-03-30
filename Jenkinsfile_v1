pipeline { 
    agent any
    stages {
        stage('Clone Git') {
            steps {
                git 'https://github.com/Anuj-2014/Pipe.git'
            }
        }
        stage('Build Code') {
            steps {
                sh "chmod 755 Prog1.py"
                sh "./Prog1.py"
            }
        }
     stage('Test Code') {
            steps {
                sh "chmod 755 Test.py"
                sh "./Test.py"
            }
        }
    } 
}
