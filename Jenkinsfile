pipeline {
    agent any 

stages{
        stage ('DOcker build image using Dockerfile'){
         steps {
            sh 'docker build -t one2onetool:latest . ' 
}
        }
    
        stage('Docker Images') { 
            steps {
                sh 'docker images'
            }
        }
      stage('docker Containers') { 
            steps {
                sh 'docker run -d -p 3000:3000 --name one2onecontainer 6c1eeedd9013 '
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
