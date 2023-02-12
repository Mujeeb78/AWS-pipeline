pipeline {
    agent any
    stages {
        stage("Checking Docker Version") {
            steps {
                retry(3){
                sh "docker --version"
                }
            }
        }
        stage("Checking GIT Version") {
            steps {
                sh "git --version"
            }
        }
        stage('Build Docker Image with build no') {
            steps {
                sh 'docker build -t apacheimage:${BUILD_NUMBER} . '
                sh 'docker images'
            }
        }
      stage('Build Docker Image with build no') {
           withCredentials([<object of type com.cloudbees.jenkins.plugins.awscredentials.AmazonWebServicesCredentialsBinding>]){
            steps {
               
               echo "aws"
           
        }
           }
      
        
    }
}
