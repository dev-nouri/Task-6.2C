pipeline{
    agent any
    environment{
        DIRECTORY_PATH="path/directory/code"
        TESTING_ENVIRONMENT="testing-environment"
        PRODUCTION_ENVIRONMENT="SIT223"
    }

    stages
    {
        stage("Build"){
            steps{
                mail to: "mnouri.2002.10@gmail.com",
                subject: "Building",
                body: "Building completed"
                echo "fetched the code from $DIRECTORY_PATH"
                echo "Building completed..."
            }
        }

        stage("Test"){
            steps{
                mail to: "mnouri.2002.10@gmail.com",
                subject: "Testing",
                body: "Testing completed"
                echo "Unit test"
                echo "iIntegrated test"
                echo "Testing completed..."
            }
        } 
    }
}
