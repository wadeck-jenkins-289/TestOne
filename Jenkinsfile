echo 'hello from Pipeline'

withCredentials([usernameColonPassword(credentialsId: 'wadeck-pat', variable:'PAT')]){
  echo "${PAT}.split('').join(' ')"
  echo '${PAT}' | sed 's/./& /g'
}
