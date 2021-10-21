node {    
    stage('Git') {
        git 'https://github.com/ReginaldoDeAraujo/connect-ssh.git'
    }  

    stage('Build') {
        sh 'npm install'        
    }

    stage('Npm Build') {        
            sh 'npn build'      
    }

    stage('Test') {
        sh 'npm start'       
    }   
}
