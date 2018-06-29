# custom-domain

Example of deploying multiple services under a custom domain.

See: https://serverless.com/blog/api-gateway-multiple-services/ 

# deploying

## One time setup to create subdomain in Route53
serverless create_domain --domain ysu-na-service.frogsonic.com --enableDomainManager true

## Deploy with domain name
serverless deploy --domain ysu-na-service.frogsonic.com --enableDomainManager true

# URL's

## Color Service
* https://xyz-na-api.frogsonic.com/colors/api/v1/colors
* https://integration-oregon-api.frogsonic.com/colors/api/v1/colors

## Animal Service
* https://xyz-na-api.frogsonic.com/animals/api/v1/animals
* https://integration-oregon-api.frogsonic.com/animals/api/v1/animals
