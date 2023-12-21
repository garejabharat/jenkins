pipeline{
    agent any
    tools {nodejs "node"}
    environment{
        imageName = "techwithbk/jenkins_apps" 
        rigistryCredential='bharatgareja'
        dockerImage = ''
    }
    stages {
       stage("Install Dependencies"){
            steps{
                sh 'npm install'
            }
       }
       stage("Tests"){
            steps{
                sh 'npm test'
            }
       }
    }
}   

