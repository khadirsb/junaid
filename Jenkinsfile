node('built-in') {
 stage('download') 
    {
    git 'https://github.com/khadirsb/devops.git'
    }
    stage('build')
    {
   sh 'mvn package'
    }
    stage('deploy') 
    {
    sh 'scp /home/ubuntu/.jenkins/workspace/pipejob/webapp/target/webapp.war ubuntu@172.31.36.84:/var/lib/tomcat9/webapps/tommy.war'
    }
    stage('test')
    {
    sh 'echo "as salamu alaikum"'
    }
    stage('delivery') 
    {
    sh 'scp /home/ubuntu/.jenkins/workspace/pipejob/webapp/target/webapp.war ubuntu@172.31.41.41:/var/lib/tomcat9/webapps/artifact.war'
    }
}

