pipeline{
    agent any
     environment{
         PATH = "/opt/maven/bin:$PATH"
               }
        stages{
          stage('GIT URL'){
              steps{
                  git url: 'https://github.com/davidmoten/maven-demo.git', branch: 'main'
                   }
          }
            stage ('MY build Jenkins Pipeline')
            {
             steps{
                 sh 'mvn clean install'
             }
          }
          
      }
      }

