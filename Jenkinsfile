pipeline {
    agent any
    stages {
        stage('UnitTest') {
            steps {
                sh "mvn -f jenkins/java-tomcat-sample/pom.xml  clean package"
                echo "Running Unitest"
            }
        }
        stage('Build') {
            steps {
                echo "Building the code"
            }
        }
        stage('DeployStaging') {
            steps {
                echo "Deploying to staging env"
            }
        }  
        stage('DeployProd') {
            steps {
                echo "Deploying to prod env"
            }
        }    
    }
}
