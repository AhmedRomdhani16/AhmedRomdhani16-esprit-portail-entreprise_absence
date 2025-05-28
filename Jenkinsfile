pipeline{
  agent any
  tools{
     maven 'maven'
  }
  stages{
    stage("Checkout code develop")
     {
        when{
        branch 'develop'
        }
        steps{
             checkout scm

        }



    }
    stage("Checkout code develop")
     {
        when{
        branch 'develop'
        }
        steps{
             sh 'mvn clean compile'

        }


    }


    stage("Checkout code QA")
     {
        when{
        branch 'qaulite'
        }
        steps{
             checkout scm

        }

     }
    stage("Checkout code prod")
     {
        when{
        branch 'master'
        }
        steps{
             checkout scm

        }


    }
  }

}