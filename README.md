Configuration for gitlab_rails with SMTP without SSL

1.Start docker compose with command:

docker-compose up -d

2.You need to know ID of your container, you can use command:

docker container ls

3.Enter in  container:

docker exec -it IDcontainer /bin/bash

4.Enter in console:

gitlab-rails console

Test message:

Notify.test_email('destination_email@address.com', 'Message Subject', 'Message Body').deliver_now
