pipeline{
 agent any
 stages{
 when{
 expression{
 $BRANCH_NAME == 'master'
 }
 }
 stage('build for master'){
 steps{
 echo ' Build for master'
 }
 }
 when{
 expression{
 $BRANCH_NAME == 'dev'
 }
 stage('Build for dev'){
 steps{
 echo 'build for dev'
 }
 }
 }
 when{
 expression{
 $BRANCH_NAME == 'feature'
 }
 }
 }
}
