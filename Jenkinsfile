node {

    stage('Checkout') {
        echo 'Downloading Metro Reservation source code'
        checkout scm
    }

    stage('Build') {
        echo 'Building Metro Reservation using Maven'
        bat 'mvn clean package'
    }

    stage('Verify') {
        echo 'Checking generated WAR file'
        bat 'dir target'
    }
}