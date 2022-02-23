/* Can use *
echo "${GIT_BRANCH.split("origin/")[1]}"
echo "${ghprbSourceBranch}"
echo "${ghprbTargetBranch}"
*/
pipeline {
    agent any
    stages{
        stage("Delete after #1"){
            steps{
                echo "Do nothing!"
            }
        }
        stage("Delete after #2"){
            steps{
                echo "Do nothing!"
            }
        }
        stage("Delete after #3"){
            steps{
                echo "Do nothing!"
            }
        }
        stage('release to master') {
            when {

                expression {
                    return CHANGE_TARGET == 'master';
                }
            }
            steps {
                echo "Do nothing!"
            }
        }
        stage('feature to develop') {
            when {

                expression {
                    return CHANGE_TARGET == 'develop';
                }
            }
            steps {
                echo "Lets code in develop!"

            }
        }
        stage("Delete after #4"){
            steps{
                echo "Do nothing!"
            }
        }
    }
}
