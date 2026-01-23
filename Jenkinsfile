pipeline {
    agent any

    environment {
        // Defining our two numbers
        NUM1 = '10'
        NUM2 = '20'
    }

    stages {
        stage('Calculation') {
            steps {
                echo "Adding ${NUM1} and ${NUM2}..."
                
                // Using a script block to do math in Groovy
                script {
                    def sum = NUM1.toInteger() + NUM2.toInteger()
                    echo "The total sum is: ${sum}"
                }
            }
        }
    }
}
