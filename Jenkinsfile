pipeline {
agent any
stages{
stage('checkout Source Repo'){
  when {
    branch 'dev'
  }
steps{
sh 'echo dev' 
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
