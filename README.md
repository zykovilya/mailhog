# MailHog docker-compose env 
- with local storage
- web ui on port 8025 with login "test"  and password "test" 
- smtp on port 2025 with login="" and password=""

 docker exec  mailhog /bin/sh -c "MailHog bcrypt login:password" > mailhog.auth


