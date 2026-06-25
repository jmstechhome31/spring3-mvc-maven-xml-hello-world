pipeline {
    agent any  
    tools {
        maven "maven3"
    }
    stages {
        stage("clone code") {
            steps {
					git credentialsId: 'github_credentials', url: 'https://github.com/jmstechhome29/spring3-mvc-maven-xml-hello-world.git'
                }
            }
        stage("mvn build") {
            steps {
                     sh "mvn clean package"
                }
            }
        }
	}


