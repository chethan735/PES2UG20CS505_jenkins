pipeline { 
agent any
 stages {
 stage('Build'){
 steps {
 sh 'g++ working.cpp'
 build job: "PES2UG20CS505-1", wait: true
 }
 }
 stage('Test'){
 steps{
 sh './a.exe'
 }
 }
 }
 post {
 failure {
 echo 'pipeline failed'
 }
 }
}
