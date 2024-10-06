pipeline {
    agent ane

    stages {
        stage('Hello'){
            steps {
                echo 'Hello from jenkins file'
            }
        }
        stage('Build app') {
             steps {
                    dotnet build 'https://github.com/DoctorVovan/JenkinsHelloWorld/blob/main/HelloWorldJenkinsTest.csproj'
             }
        }
        stage('Run app'){
            steps {
                 dotnet run 'https://github.com/DoctorVovan/JenkinsHelloWorld/blob/main/bin/Debug/HelloWorldJenkinsTest.exe'
            }
        }
    }
}
