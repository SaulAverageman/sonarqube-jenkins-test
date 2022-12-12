pipeline{
    agent any
    tools{
        maven 'MAVEN'
    }

    stages{
        stage('run sonarqube'){
            steps{
                script{
                    withSonarQubeEnv('sonarqube-server'){
                        sh 'mvn sonar:sonar'
                    }
                }
            }
        }
    }
    
}