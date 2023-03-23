pipeline {
  agent any
  tools { 
        maven 'maven_2_39_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=abraham -Dsonar.organization=abraham -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=0d77e0266e34ef97a60dc39d2e382f1fdad269c2'
			}
        } 
  }
}
