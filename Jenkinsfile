pipeline{
  agent any
  stages{
    stage('Chekout'){
      steps{
        git branch: 'Main',
          url:'https://github.com/Hacker-Hima/jenkins-practice-1.git'
      }
    }
    stage('Compile'){
      steps{
        bat 'javac AddingTwoNum.java'
      }
    }
    stage('Execute'){
      steps{
        bat 'java AddingTwoNum'
      }
    }
  }
post{
  success{
    echo 'Programm Executed Successfully'
  }
  failure{
    echo 'ProgramExecution Failed'
  }
  always{
    echo 'PipeLine Completed'
  }
}
}
    
