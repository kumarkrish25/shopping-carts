pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
   tools{
       maven 'kkdojomaven' 
    }
    

    stages{
        stage('build'){
            steps{
                echo 'this is the build job'
                sh 'mvn compile'
               
            }
        }
        stage('test'){
            steps{
                echo 'this is the second job'
                sh 'mvn clean test'
                
            }
        }
        stage('package'){
            steps{
                echo 'this is the package job'
                sh 'mvn run package'
        }
    }
}    
    post{
        always{
            echo 'this is my second pipeline has completed... Shopping Cart'
        }
        
    }
    
}
