node {
    
	

    env.AWS_ECR_LOGIN=true
    def newApp
    def registry = 'https://github.com/ReginaldoDeAraujo/connect-ssh'
    def registryCredential = 'dockerhub'
    def install() {
        steps.stage('Get Dependencies') {
            steps.sh "yarn install"
        	}
    	}
    def build() {
        steps.stage('NPM Build') {
            steps.sh "yarn run build"
       		 }
    	}
	
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
