pipeline {
    agent any 
    parameters { 
         string(defaultValue: "1.0.0.0", description: 'Image version ', name: 'imageversion')
    
    }

stages{
        stage ('DOcker build image using Dockerfile'){
         steps {
            sh 'docker build -t one2onetool:${imageversion} . ' 
}
        }
    
        stage('Docker Images') { 
            steps {
                sh 'docker images'
            }
        }
      stage('docker Containers') { 
            steps {
                sh 'docker run -d -p 3000:3000 --name one2onecontainer one2onetool:${imageversion} '
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
