pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
/*    tools{
       maven 'Maven 3.6.3' 
    }
*/    

    stages{
        stage('one'){
            steps{
                echo 'this is the first job'
                sleep 4
            }
        }
        stage('two'){
            steps{
                echo 'this is the second job'
                sleep 9
            }
        }
        stage('three'){
            steps{
                echo 'this is the third job'
                sleep 7
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}
