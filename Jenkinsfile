pipeline {
agent any
stages {
stage('Build') {
steps {
echo 'Build World'
}
}
stages('Deploy') {
steps {
echo 'Test World'
}
}
stage('Test') {
steps {
echo 'Deploy World'
}
}
}
post
{
always
{
emailtext body: 'Summary', subject: 'Pipeline Status', to: 'tusharvitole.scoe.entc@gmail.com'
}
}
}
