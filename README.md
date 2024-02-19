
# Prérequis 
- php 
- composer
- environnement
- git


# Installation 
- docker (https://www.docker.com/get-started/)
	- test : ```bash docker -v ```
	
- Postman (https://www.postman.com/downloads/)
	- adresse environnement : **TODO**

- MySQL Workbench (https://dev.mysql.com/downloads/workbench/)
	



## Clone project :
```bash
git clone --branch <tag> <repo>
git clone --branch env/preprod  https://git.dotsafe.fr/sauv-life/backend-sauvlife.git
``` 
 
- docs : https://www.atlassian.com/fr/git/tutorials/setting-up-a-repository/git-clone




## Changement .env.test
```.env
APP_NAME="[local] SauvLife"
APP_ENV=test
APP_KEY=base64:Yfmhggfb2u7c+g3dqWdN2FVYVBVW0Rz7nDiXVuLbySo=
APP_DEBUG=true
APP_URL=https://local.sauv.life

MOBILE_SCHEME=sauvlife://

LOG_CHANNEL=stack
LOG_DEPRECATIONS_CHANNEL=null
LOG_LEVEL=debug

DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=sauvlife_test
DB_DATABASE_legacy=sauvlife
DB_USERNAME=test
DB_PASSWORD="test"
DB_DATABASE_LEGACY=sauvlife

SMS_DRIVER=SAUVLIFE
BROADCAST_DRIVER=pusher
CACHE_DRIVER=redis
FILESYSTEM_DISK=local
QUEUE_CONNECTION=redis
SESSION_DRIVER=redis
SESSION_LIFETIME=525600

REDIS_HOST=redis
REDIS_PASSWORD=null
REDIS_PORT=6379
HORIZON_PREFIX=sauvlife_horizon:

TRUSTED_PROXY_HEADERS=HEADER_X_FORWARDED_AWS_ELB

MAIL_MAILER=smtp
MAIL_HOST=mailhog
MAIL_PORT=1025
MAIL_USERNAME=root
MAIL_PASSWORD=root
MAIL_ENCRYPTION=tls
MAIL_FROM_ADDRESS=noreply@application.sauv.org
MAIL_FROM_NAME="No-Reply ${APP_NAME}"
# MAIL_TO_OVERRIDE=sauvlife.testing@big-boss-studio.com

# PUSHER_APP_ID=1372832
# PUSHER_APP_KEY=
# PUSHER_APP_SECRET=
# PUSHER_APP_CLUSTER=eu
PUSHER_APP_ID=1570000
PUSHER_APP_KEY=
PUSHER_APP_SECRET=
PUSHER_APP_CLUSTER=eu

LIGHTHOUSE_CACHE_ENABLE=0
LIGHTHOUSE_BROADCASTER=pusher
LIGHTHOUSE_SUBSCRIPTION_VERSION=2
LIGHTHOUSE_SUBSCRIPTION_EXCLUDE_EMPTY=true
LIGHTHOUSE_SUBSCRIPTION_STORAGE_TTL=1800

LPQ_CACHE_PREFIX=sauvlife_apq
LPQ_CACHE_TTL=0
LPQ_CACHE_MAX_AGE=86400

NOVA_LICENSE_KEY=

BUGSNAG_API_KEY=

# GOOGLE_API_KEY=
GOOGLE_API_KEY=

NEVERBOUNCE_API_KEY=

SMS_MODE_API_KEY=

# ----- SMULLER
TWILIO_ACCOUNT_SID=
TWILIO_AUTH_TOKEN=
TWILIO_SMS_FROM=
TWILIO_API_KEY=
TWILIO_API_SECRET=
# ----- SAUVLIFE
# TWILIO_ACCOUNT_SID=
# TWILIO_AUTH_TOKEN=
# TWILIO_SMS_FROM=
# TWILIO_API_KEY=
# TWILIO_API_SECRET=

```




## Apport .env
```.env
APP_NAME="[local] SauvLife"
APP_ENV=local
APP_KEY=base64:Yfmhggfb2u7c+g3dqWdN2FVYVBVW0Rz7nDiXVuLbySo=
APP_DEBUG=true
APP_URL=https://local.sauv.life

MOBILE_SCHEME=sauvlife://

LOG_CHANNEL=stack
LOG_DEPRECATIONS_CHANNEL=null
LOG_LEVEL=debug

DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=sauvlife
DB_DATABASE_legacy=sauvlife
DB_USERNAME=root
DB_PASSWORD="root"
DB_DATABASE_LEGACY=sauvlife

SMS_DRIVER=SAUVLIFE
BROADCAST_DRIVER=pusher
CACHE_DRIVER=redis
FILESYSTEM_DISK=local
QUEUE_CONNECTION=redis
SESSION_DRIVER=redis
SESSION_LIFETIME=525600

REDIS_HOST=redis
REDIS_PASSWORD=null
REDIS_PORT=6379
HORIZON_PREFIX=sauvlife_horizon:

TRUSTED_PROXY_HEADERS=HEADER_X_FORWARDED_AWS_ELB

MAIL_MAILER=smtp
MAIL_HOST=mailhog
MAIL_PORT=1025
MAIL_USERNAME=root
MAIL_PASSWORD=root
MAIL_ENCRYPTION=tls
MAIL_FROM_ADDRESS=noreply@application.sauv.org
MAIL_FROM_NAME="No-Reply ${APP_NAME}"
# MAIL_TO_OVERRIDE=sauvlife.testing@big-boss-studio.com

# PUSHER_APP_ID=1372832
# PUSHER_APP_KEY=9e0c10ab87f468946171
# PUSHER_APP_SECRET=421a1579a8012e50b565
# PUSHER_APP_CLUSTER=eu
PUSHER_APP_ID=1570000
PUSHER_APP_KEY=e201fa11fb7e9d576bd8
PUSHER_APP_SECRET=71068a97a918a5722864
PUSHER_APP_CLUSTER=eu

LIGHTHOUSE_CACHE_ENABLE=0
LIGHTHOUSE_BROADCASTER=pusher
LIGHTHOUSE_SUBSCRIPTION_VERSION=2
LIGHTHOUSE_SUBSCRIPTION_EXCLUDE_EMPTY=true
LIGHTHOUSE_SUBSCRIPTION_STORAGE_TTL=1800

LPQ_CACHE_PREFIX=sauvlife_apq
LPQ_CACHE_TTL=0
LPQ_CACHE_MAX_AGE=86400

NOVA_LICENSE_KEY=8Us30BIXPTiL7TGf0RvELi9VPsoujR5tTg7Yn7pjEx2SNRdVJg

BUGSNAG_API_KEY=53dec4485165de708e978f8182c6c0ff

# GOOGLE_API_KEY=AIzaSyAIUSKnPo8VJAvH_uT7btpwnlBXHIfqsuc
GOOGLE_API_KEY=AIzaSyBNjpeR1wvVCSyxE0en6P00HLXzraz1000

NEVERBOUNCE_API_KEY=private_09d708447d0f9b1cda0d3d8e1cd6e000

SMS_MODE_API_KEY=a2LCP8D0Kbk4xJVKkQR3kdlQZjyMu000

# ----- SMULLER
TWILIO_ACCOUNT_SID=AC9f7d622825d01669d5e18849aa0e085000000
TWILIO_AUTH_TOKEN=d30a42ff6c13465b5bf17b5132755f37
TWILIO_SMS_FROM=+19362376971
TWILIO_API_KEY=SKc4c767bf838abd51114bc83edb0860be
TWILIO_API_SECRET=MiDoYxhHGUpP79QLI014d3L4MgTKljyc
# ----- SAUVLIFE
# TWILIO_ACCOUNT_SID=AC034129d9f2fe05f576b61421166836e8
# TWILIO_AUTH_TOKEN=d28562b8f0113daec8b9f54279c9da88
# TWILIO_SMS_FROM=+15077044988
# TWILIO_API_KEY=SK30e8ce3fc35bbfa0b09d0ebb2fe5ce21
# TWILIO_API_SECRET=EUfaFf9RlqagoXfhgMMQ9R2m1oigOw82

```



## Lancement 1er build docker

Lancement du premier build depuis invite de commande administrateur pour palier au risque de timeOUT
```bash docker compose build ```
	
	
### Problemes docker Horizon
Code erreur
	horizon-1  | /usr/local/bin/docker-php-entrypoint: 9: exec: wait: not found
	horizon-1 exited with code 127


#### Solution Temporaire
  Commenter les lignes composer Horizon

	Fichier docker-compose.yml :
	```yml
		  # horizon:
		  #   build:
		  #     context: ./
		  #     dockerfile: Dockerfile
		  #   command: [ "wait", "backend:80", "-t", "0", "--", "php", "artisan", "horizon" ]
		  #   depends_on:
		  #     - backend
		  #   restart: unless-stopped
		  #   volumes:
		  #     - "./:/web/html:cached"
		  #     - "~/.composer/cache/:/root/.composer/cache:cached"
		  #   networks:
		  #     - sauvlife
	```
		  
		  
#### Solution :

**TODO**
	
	
### Problemes docker cache
=> CANCELED [backend internal] load build context  

```bash docker system prune -a ```


	
## Lancement docker
Lancement de docker depuis invite de commande administrateur pour palier au risque de timeOUT
	```bash docker compose up ```
			
### Problemes install Failed
Alterner 
```bash docker compose down ```

```bash docker compose up ```
afin d'installer les dépendances peu à peu
	
## connnection docker back
```bash docker compose exec backend bash ```
	
## connnection docker mysql	
```bash 
  docker compose exec mysql bash 
  mysql --host=mysql --user=root --password=root
```
	
## Lancement test

```bash 
  docker compose exec backend bash 
  vendor/bin/codecept run --steps 
```
	
	
### Probleme base BBD test non créé
#### Verification .env & .env.test 
	```bash
	  DB_CONNECTION=mysql
	  DB_HOST=mysql
	  DB_PORT=3306
	  DB_DATABASE=sauvlife_test
	  DB_DATABASE_legacy=sauvlife
	  DB_USERNAME=root
	  DB_PASSWORD="root"
	  DB_DATABASE_LEGACY=sauvlife
	```
	```bash
	  DB_CONNECTION=mysql
	  DB_HOST=mysql
	  DB_PORT=3306
	  DB_DATABASE=sauvlife
	  DB_DATABASE_legacy=sauvlife
	  DB_USERNAME=root
	  DB_PASSWORD="root"
	  DB_DATABASE_LEGACY=sauvlife
	```
	
#### Ajout ligne dans docker-compose.yml 

```bash php artisan migrate --force --env=test; ```


