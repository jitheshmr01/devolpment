node('node1')
{
    mavenhome = tool name:"maven3.6.3"
    
    
stage('clone code from github'){
    git branch: 'development', credentialsId: '8b33c26e-0e56-45ab-b0a8-cff85b1d9b56', url: 'https://github.com/jitheshmr01/devolpment.git'
}    
stage('creating a package'){
    sh "${mavenhome}/bin/mvn clean package"
}
/*  
stage('creating artifactorsh "${mavenhome}/bin/mvn clean deploy"y'){
    sh "${mavenhome}/bin/mvn clean deploy"
}
stage('deploy into tomacat server'){
    sshagent(['b30785b1-df07-404f-a0b3-2647a7150532']) {
      sh "scp -o StrictHostKeyChecking=no target/maven-web-application.war ec2-user@15.206.164.46:/opt/apache-tomcat-9.0.43/webapps/"
}
}*/
  
}
