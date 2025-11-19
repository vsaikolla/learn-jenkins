pipeline {
    agent {
        label 'AGENT-1'
    }
    options{
        timeout(time: 30, unit: 'MINUTES')
    }
    stages {
        stage('Build') { 
            steps {
                sh 'echo this is from build' 
            }
        }
        stage('Test') { 
            steps {
                sh 'echo this is from test' 
                sh 'sleep 10'
            }
        }
        stage('Deploy') { 
            steps {
                sh 'echo this is from deploy'  
            }
        }
    }
}