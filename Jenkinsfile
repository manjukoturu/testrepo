pipeline { 
    agent any 
    stages {
        stage('git clone') { 
            steps { 
                git 'http://192.168.75.92:8080/gitbucket/git/manju/maventest.git' 
            }
        }
        stage('mvn compile'){
            steps{
                sh 'mvn compile'
            }
        }
        stage('mvn test'){
         steps{
             sh 'mvn test'
         }
        }
        stage('mvn package'){
         steps{
             sh 'mvn package'
         }
        }
    }  
}
