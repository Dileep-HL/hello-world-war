pipeline{
      agent none
      stages{
      stage('check out'){
                  steps{
                  sh "rm -rf hello-world-war"
                  sh "git clone https://github.com/Dileep-HL/hello-world-war.git"
                  }
                  }
      stage('build'){
      steps{
      sh "pwd"
      sh "ls"
      sh "cd hello-world-war"
      sh "docker build -t dileep288/docwarimage:1.0 ."
      }
      }
       stage('publish'){
                  steps{
                        sh "docker login -u dileep288 -p 1019@Lmsdin"
                        sh "docker push  dileep288/docwarimage:1.0"
                  }
            }
            
      }
      }
