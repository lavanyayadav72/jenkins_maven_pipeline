pipeline{
    agent any
    triggers {
        githubPush()
    }
    stages {
	stage('code checkout') {
            steps {
		git(
                    url: 'git@github.com:lavanyayadav72/jenkins_maven_pipeline.git'
                    credentialsId: 'github-ssh-key'
                   )
            }
       }
    }
}
