pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=azertyuio -Dsonar.organization=project -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=9d2c0be54efce7b5710876da610384ccf163e44f'
			}
        } 
  }
}
