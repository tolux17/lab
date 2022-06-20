pipeline {
    agent any

    environment {

        BRANCH_NAME="main"
    }

    stages {
        stage ('Julius') {

            steps {

                echo "My name is Julius"
            }
        }

        stage ('Tchami') {

            steps {

                echo "My name is Tchami"
            }
        }

        stage ('Deploy') {

            when {

                expression {

                    BRANCH_NAME == "jobs"
                }
            }

            steps {

                echo 'we are deploying'
            }
        }
    }
}