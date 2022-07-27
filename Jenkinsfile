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
      stage('Test') { 
            steps {
                sh 'docker ps '
            }
        }
stage('Delpoy nodejs application') { 
            steps {
                sh 'echo "deploying application.."'
    }
}
    
}
    // post{
     //   always{
      //      mail to: "raob6730@gmail.com",
       //     subject: "Test Email",
        //    body: "Test"
        //}
    //}

}
