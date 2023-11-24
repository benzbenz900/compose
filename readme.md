# config install
```sh
# 11111
apt install awscli
aws configure

AWS Access Key ID [None]: AKIAURXCKNYCYSNQ6ZVR
AWS Secret Access Key [None]: 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
Default region name [None]: ap-southeast-1

# 22222
aws ecr get-login-password --region ap-southeast-1 | docker login --username AWS --password-stdin 312933510661.dkr.ecr.ap-southeast-1.amazonaws.com

# compose == v2.23.3
sudo curl -L "https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-$(uname -s)-$(uname -m)" -o /usr/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
docker-compose --version


# 3333
docker compose -p ntpdpa config -o BUILD_TAMPLATE.yaml
docker-compose -f BUILD_TAMPLATE.yaml up -d
```
# image
312933510661.dkr.ecr.ap-southeast-1.amazonaws.com/onefence-usermanagement-api:NT-dev1.0
312933510661.dkr.ecr.ap-southeast-1.amazonaws.com/onefence-data-mapping-service:NT-dev1.0
312933510661.dkr.ecr.ap-southeast-1.amazonaws.com/onefence-consent-v2-api:NT-dev1.0
312933510661.dkr.ecr.ap-southeast-1.amazonaws.com/onefence-log:NT-dev1.0
312933510661.dkr.ecr.ap-southeast-1.amazonaws.com/onefence-keycloak-container-theme:NT-dev1.0
312933510661.dkr.ecr.ap-southeast-1.amazonaws.com/onefence-notification-sns-websocket-sqs:NT-dev1.0
312933510661.dkr.ecr.ap-southeast-1.amazonaws.com/onefence-comment-service:NT-dev1.0
312933510661.dkr.ecr.ap-southeast-1.amazonaws.com/onefence-file-management:NT-dev1.0

# url
http://10.44.66.50/auth/login
http://10.44.66.50/data-mapping
http://10.44.66.50/consentv2
http://10.44.66.50/organization
http://10.44.66.50/log
http://10.44.66.50/s3
http://10.44.66.50/s3/admin
http://10.44.66.50/usermanagement
http://10.44.66.50/notification-service
http://10.44.66.50/comment_service
http://10.44.66.50/file_management