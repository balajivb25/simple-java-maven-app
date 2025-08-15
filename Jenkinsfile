pipeline {
    agent any
    tools {
        maven 'Maven3.9.9'   // This name must match the one in Jenkins > Manage Jenkins > Tools > Maven installations
        jdk 'JDK17'          // This name must match the one in Jenkins > Manage Jenkins > Tools > JDK installations
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
