node{

stage('SCM'){
//git clone
git 'https://github.com/GitPracticeRepo/spring-petclinic.git'
}
stage('build the package'){
//mvn package
sh  'mvn package'
}
stage('show the test results'){
//test reports
junit 'target/surefire-reports/*.xml'
}
stage('archival'){
//archiving artifacts
archive 'target/*.jar'
}

}