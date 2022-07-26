pipeline {
    agent any 

stages{
        stage ('Install Dependcies'){
         steps {
            sh 'npm install' 
}
        }
    
        stage('Test') { 
            steps {
                sh 'echo "testing application.."'
            }
        }
stage('Delpoy nodejs application') { 
            steps {
                sh 'echo "deploying application.."'
    }
}
    
}
     post {
        always {
            emailext body: 'A Test EMail', recipientProviders: [[$class: 'DevelopersRecipientProvider'], [$class: 'RequesterRecipientProvider']], subject: 'Test'
        }
    }
}
