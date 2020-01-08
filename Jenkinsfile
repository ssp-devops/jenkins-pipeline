node(){
    stage('Build'){
        echo " Build Job is Succcsful"
    }
    stage('Deploy'){
        echo "Deploy Job is Succesful"
    }
    stage('Test'){
        echo "Test Job is Succesful"
        
    }
    stage('Release'){
        echo " Release Job is Succesful ============"
    }
    stage('Notify'){
        echo " Notify Job is Succesful"
        slackSend channel: 'jenkins-notify', color: 'good', message: "Success ${env.JOB_NAME} ${env.BUILD_NUMBER} (<${env.BUILD_URL}|Open>)", teamDomain: 'sspcloudpro', tokenCredentialId: 'sspcloudslacktoken', username: 'jenkins'
    }
}

