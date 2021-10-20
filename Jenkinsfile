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
	stage('Npm Install And Build') {
    steps {
      sh 'npm install'
      sh 'npm run build'
	}
    }
}
