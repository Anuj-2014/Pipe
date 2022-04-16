pipeline { 
    agent any
    stages {
        stage('Clone Git') {
            steps {
                git branch: 'main',
    credentialsId: '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',
    url: 'https://github.com/Anuj-2014/Pipe'
//                 git 'https://github.com/Anuj-2014/Pipe'
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
