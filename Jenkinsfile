echo 'hello from Pipeline'

withCredentials([usernameColonPassword(credentialsId: 'wadeck-pat', variable:'PAT')]){
  echo "${PAT}.split('').join(' ')"
  sh("echo '${PAT}' | sed 's/./& /g'")
  sh '''
     echo '${PAT}' | sed 's/./& /g'
     '''
}
