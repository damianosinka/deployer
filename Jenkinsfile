
pipeline {
    agent any

    parameters {
        choice(choices: ['pp-liabilities', 'pp-credits'], description: 'What MS?', name: 'ms')
	  choice(choices: ['dev', 'uat', 'pp'], description: 'What environment?', name: 'env')
        choice(choices: ['kluster1', 'kluster2', 'kluster3'], description: 'What cluster?', name: 'cluster')
    }

    stages {
        stage("deploy") {
            steps {
                echo "Deploing ${params.ms} to environment ${params.env} in cluster ${params.cluster}"
            }
        }
    }
}
