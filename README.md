# MailHog docker-compose env 
- with local storage
- web ui on port 8025 with login "test"  and password "test" 
- smtp on port 2025 with login="" and password=""

## Change login and password

 `printf "login:" > mailhog.auth`
 
 `printf "$(sudo docker exec  mailhog /bin/sh -c "MailHog bcrypt password")" >> mailhog.auth`
  mailhog - name of docker container mailhog

 `cat mailhog.auth`
