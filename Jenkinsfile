pipeline {
  agent any

  parameters {
    // Define your parameters here
    // For example, a string parameter and a choice parameter
    string(name: 'VERSION', defaultValue: '1.0', description: 'Enter the version number')
    choice(name: 'ENVIRONMENT', choices: ['dev', 'staging', 'production'], description: 'Select the target environment')
  }

  environment {
    // Define your environment variables here
    // For example, setting a custom variable
    MY_VARIABLE = 'some value'
  }

  stages {
    stage('Build') {
      steps {
        // Add build steps here
        // For example, running a shell command
        sh 'echo "Building the project..."'
      }
    }

    stage('Test') {
      steps {
        // Add test steps here
        // For example, running test scripts or commands
        sh 'echo "Running tests..."'
      }
    }

    stage('Deploy') {
      steps {
        // Add deployment steps here
        // For example, deploying to a specific environment based on the selected choice parameter
        sh 'echo "Deploying to ${ENVIRONMENT} environment..."'
      }
    }
  }
}
