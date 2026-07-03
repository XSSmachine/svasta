curl -s -o /dev/null -w "%{http_code}\n" \
  -u "username:TvojaLozinka" \
  "https://pbznexus.sit.pbz.hr/repository/pbz-composer-eap-group/packages.json"
