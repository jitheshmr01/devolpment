node
{
def mavenHome = tool name: "maven3.6.3"
    
stage('CodeCheckout')
{
git branch: 'development', credentialsId: '8b33c26e-0e56-45ab-b0a8-cff85b1d9b56', url: 'https://github.com/jitheshmr01/devolpment.git'
}
stage('Build')
{
sh "${mavenHome}/bin/mvn clean package"
}
/* stage('sonarqubereport')
{
sh "${mavenHome}/bin/mvn sonar:sonar"    
}
stage('nexus artifacts')
{
sh "${mavenHome}/bin/mvn deploy"
}*/

}
