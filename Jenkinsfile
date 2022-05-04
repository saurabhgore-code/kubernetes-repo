podTemplate(containers: [
    containerTemplate(name: 'apache-container', image: 'httpd', command: 'sleep', args: '99d')
  ]) 
{
node(server) {
        stage('Get the project') {
            git 'https://github.com/saurabhgore-code/kubernetes-repo.git'
            container('apache') {
                stage('run apache container') {
                    sh 'echo my name is sagore'
                }
            }
        }
}
}
