pipeline {
    agent any 

stages{
        stage ('Install Dependcies'){
         steps {
            sh 'docker build -t one2onetool:latest . ' 
}
        }
    
        stage('Test') { 
            steps {
                sh 'docker images'
            }
        }
      stage('docker stage') { 
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
