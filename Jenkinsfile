pipeline{
    agent any
    triggers {
        githubPush()
    }
    stages {
	stage('code checkout') {
            steps {
              checkout([$class: 'GitSCM',
               branches: [[name = */main]],
               userRemoteConfigs: [[  
	            url: 'git@github.com:lavanyayadav72/jenkins_maven_pipeline.git',
                    credentialsId: 'github-ssh-key'
                   ]]
             ])    
            }
       }
    }
}
