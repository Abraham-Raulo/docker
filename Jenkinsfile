pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=abraham -Dsonar.organization=abraham -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=35735ffdd1ee249999926df7f2a39434c363fa92'
			}
        } 
  }
}
