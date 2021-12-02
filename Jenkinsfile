pipeline {
agent any
stages{
stage('checkout Source Repo'){
  when {
    branch 'dev'
  }
steps{

sh 'echo dev' 

sh 'echo main'

}
}
  stage('qa'){
    when{
    branch 'qa'
    }
    steps{
    sh 'echo qa'
    }
  
  }
}
}
