
## About Laravel

These confguration files is <br />
from [Repo] https://github.com/emad-zaamout/Laravel-Complete-Dockerization <br />
from [Video] https://www.youtube.com/watch?v=WahJ91Nrgn0 <br />
but i did some adjusts to suits me.




- just copy them and run
- docker-compose build && docker-compose up -d
- you can also edit docker files but first, remove old container with this
- docker-compose rm -s
- then build and compose up again
- you might face a permission issue for the entrypoint.sh file just run
- sudo chmod 775 docker/entrypoint.sh
- don't forget the update your .env file, compare it with the .env i've uploaded
- if you got error at composer install, remove composer.lock file
- if you want to run queue:listen 
- docker exec -it container_name php artisan queue:listen
- by the way, I don't see that's suits a production environment, if you want to run this as production change php image with nginx image or apache image
