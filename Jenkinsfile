pipeline{
  agent any
  stages{
    stage("master branch")
    {
      steps{
        git 'https://github.com/Harikrushn96/mavenproject.git'
      }
    }
    stage("dev branch")
    {
      steps{
        git branch: 'dev', url: 'https://github.com/Harikrushn96/mavenproject.git'
      }
    }
    stage("build")
    {
      steps{
        bat "mvn clean install"
      }
    }
  }
}
    
    
