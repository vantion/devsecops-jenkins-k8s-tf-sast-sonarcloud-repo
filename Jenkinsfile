pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sonarcloudwebapp -Dsonar.organization=sonarcloudwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=200c5ece8e536e0b89f132967f063be7a26ab804'
			}
        } 
  }
}
