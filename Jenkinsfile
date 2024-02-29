pipeline {
    agent any  // Uses any available agent

    tools {
        // Explicitly defines Node.js version (replace "16.19.0" with desired version)
        nodejs "node"
    }

    stages {
        stage('Install dependencies') {
            steps {
                sh 'npm install'  // Installs dependencies from package.json 
            }
        }
                stage('Dev') {
            steps {
                sh 'npm run dev'  // Example command (replace with your desired task)
            }
        }
        stage('build') {
            steps {
                sh 'npm run build'  // Example command (replace with your desired task)
                sh 'rpm run build --report'
            }
        }
        // Add additional stages for your specific workflow (e.g., build, test, deploy)
        // Replace "Example" with meaningful stage names and relevant steps within each stage.
        stage('Example') {
            steps {
                sh 'npm config ls'  // Example command (replace with your desired task)
            }
        }
    }
    
}
