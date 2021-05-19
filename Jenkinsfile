pipeline{
agent {
label 'NODEJS'
}
     stages{
        stage('Download dependencies'){
        steps {
        sh '''
        mvn clean package
        '''
        }
        }
       stage('Prepare Artifacts'){
                steps {
                sh '''
                zip -r users.zip users-api-0.0.1.jar
                '''
                }
                }
        stage('upload artifacts'){
        steps{
        sh '''
        curl -v -u admin:admin123 --upload-file /home/ubuntu/workspace/users.zip http://192.168.0.52:8081/repository/users/users.zip
        '''
        }}
       }
     }
