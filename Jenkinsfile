pipeline {
  agent any
  tools { 
        maven 'Maven_3_9_11'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggyappjothi -Dsonar.organization=buggyappjothi -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=16df90e9d5fe50cd6af51f55349a22934604ce50'
			}
        } 
  }
}
