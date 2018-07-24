team-wiki
============


### installation guide


process environments list

#### basic envs
* NODE_ENV: production|development|test
* SITE_NAME: site name, for some display item. like page title or displayed merchant name for payment
* DATABASE_URL: only works in production env

#### payment envs
* ALIPAY_APPID: alipay app id
* ALIPAY_PUBKEY: alipay public key **content**, if not set will read content from `config/ALIPAY_PUBKEY.pem`
* ALIPAY_PRIVKEY: alipay merchants priv key **content**, if not set will read content from `config/ALIPAY_MERCHANT_PRIVKEY.pem`
* ALI_NOTIFY_URL: alipay default notifiy url, no default value
 
#### loggin envs
* LOG_FIELNAME_${category_name_in_big_case}: log file path or different `log4js-node` categories.

#### CORS
* CORS_ORIGIN: if not set, request must have header "Origin: {your_domain}"
* CORS_ALLOW_METHODS: default is 'GET,HEAD,PUT,POST,DELETE,PATCH'
* CORS_EXPOSE_HEADERS
* CORS_ALLOW_HEADERS
> `credentials` is fixed to `true`
