/*def targetBranch = env.CHANGE_BRANCH
pipeline {
    agent any
    
    stages {
            
        stage('Master') {
            when {
                expression {
                    return targetBranch == 'master';
                }
            }
            steps {
                echo "**** MASTER ****"
                build job: 'Test'
            }
        }
        
        stage('Develop') {
            when {
                    expression {
                        return targetBranch == 'develop';
                    }
            } 
            steps {
                    echo "**** DEVELOP ****"
            }
        }
        
    }
}*/
pipeline {
    agent any
     stages { 
        stage('Test') {
            steps{
                expression {
                    branchName = env.CHANGE_TARGET
                    return branchName
                    echo branchName
                }
            }
        }     
     }
}
