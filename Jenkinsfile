pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=lebio -Dsonar.organization=lebio -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=a32ea350d21f5ab390962da573543f355cf2af5e'
			}
        } 
  }
}
