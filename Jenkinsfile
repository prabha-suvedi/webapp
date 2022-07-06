node {

stage('SCM') {

checkout scm

}

stage('SonarQube Analysis') {

def scannerHome = tool 'SonarQube';

withSonarQubeEnv() {

bat "${scannerHome}/bin/sonar-scanner -Dsonar.projectKey=testapp2"

}

}

}
