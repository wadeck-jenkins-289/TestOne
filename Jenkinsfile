echo 'hello from Pipeline'

withCredentials([usernameColonPassword(credentialsId: 'wadeck-pat', variable:'PAT')]){
  echo 'attempt 1'
  echo "${PAT.split('').join(' ')}"
  echo 'attempt 2'
  sh("echo '${PAT}' | sed 's/./& /g'")
  echo 'attempt 3'
  sh '''
     echo '${PAT}' | sed 's/./& /g'
     '''
}
