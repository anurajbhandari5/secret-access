pipeline {
agent any
stages{
stage('checkout Source Repo'){
steps{
withCredentials([string(credentialsId: 'pgithubtoken', variable: 'secret')]) {
script {
def creds = readJSON text: secret
env.username= creds['username']
env.pat= creds['pat']
//env.AWS_REGION = 'us-east-1' // or whatever
}
}
sh "echo ${env.username}"
sh "echo ${env.pat}"// or whatever



}
}
}
}
