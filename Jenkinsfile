node {
    
	

    env.AWS_ECR_LOGIN=true
    def newApp
    def registry = 'https://github.com/ReginaldoDeAraujo/connect-ssh'
    def registryCredential = 'dockerhub'
	
	stage('Git') {
		git 'https://github.com/ReginaldoDeAraujo/connect-ssh'
	}
	stage('Build') {
		sh 'npm install'
	}
	stage('Test') {
		sh 'npm test'
	}
	stage('Npm Build') {   
      		sh 'npm run build'	
   	}
}
