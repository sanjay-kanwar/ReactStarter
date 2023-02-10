curl \
-d "client_id=admin-cli" \
-d "username=admin" \
-d "password=admin" \
-d "grant_type=password" \
"http://localhost:8080/realms/master/protocol/openid-connect/token"


./oauth2-proxy \
oauth2-proxy --http-address=0.0.0.0:4180 \
oauth2-proxy --cookie-secure=false \
oauth2-proxy --cookie-secret=1234567890123456 \
oauth2-proxy --upstream="http://localhost:3000" \
oauth2-proxy --provider=keycloak \
oauth2-proxy --client-id=oauth2-proxy \
oauth2-proxy --client-secret=KpMpLk8C97Ez6WofBnvIQN8ilcPJSbpf \
oauth2-proxy --insecure-oidc-allow-unverified-email=true \
oauth2-proxy --redirect-url="http://localhost:4180/oauth2/callback" \
oauth2-proxy --oidc-issuer-url="http://localhost:8080/realms/master"
oauth2-proxy --redeem-url="http://localhost:8080/realms/master/protocol/openid-connect/token" \
oauth2-proxy --login-url="http://localhost:8080/realms/master/protocol/openid-connect/auth" \
oauth2-proxy --profile-url="http://localhost:8080/realms/master/protocol/openid-connect/userinfo" \
oauth2-proxy --validate-url="http://localhost:8080/realms/master/protocol/openid-connect/userinfo" \
oauth2-proxy --email-domain="*"

./oauth2-proxy \
oauth2-proxy --http-address=0.0.0.0:4180 \
oauth2-proxy --cookie-secure=false \
oauth2-proxy --cookie-secret=1234567890123456 \
oauth2-proxy --upstream="http://localhost:3000" \
oauth2-proxy --provider=keycloak-oidc \
oauth2-proxy --client-id=oauth2-proxy \
oauth2-proxy --client-secret=KpMpLk8C97Ez6WofBnvIQN8ilcPJSbpf \
oauth2-proxy --oidc-issuer-url="http://localhost:8080/realms/master" \
oauth2-proxy --insecure-oidc-allow-unverified-email=true \
oauth2-proxy --redirect-url="http://localhost:4180/oauth2/callback" \
oauth2-proxy --oidc-issuer-url="http://localhost:8080/realms/master" \
oauth2-proxy --redeem-url="http://localhost:8080/realms/master/protocol/openid-connect/token" \
oauth2-proxy --login-url="http://localhost:8080/realms/master/protocol/openid-connect/auth" \
oauth2-proxy --profile-url="http://localhost:8080/realms/master/protocol/openid-connect/userinfo" \
oauth2-proxy --validate-url="http://localhost:8080/realms/master/protocol/openid-connect/userinfo" \
oauth2-proxy --email-domain="*"



 ./oauth2-proxy \
oauth2-proxy --http-address=0.0.0.0:4180 \
oauth2-proxy --cookie-secure=false \
oauth2-proxy --cookie-secret=1234567890123456 \
oauth2-proxy --upstream="http://localhost:3000" \
oauth2-proxy --provider=keycloak-oidc \
oauth2-proxy --client-id=oauth2-proxy \
oauth2-proxy --client-secret=XjAzrZJ7enpo9bmlOXjL3RfMeGzBcZBF \
oauth2-proxy --oidc-issuer-url="http://localhost:8080/realms/master" \
oauth2-proxy --insecure-oidc-allow-unverified-email=true \
oauth2-proxy --redirect-url="http://localhost:4180/oauth2/callback" \
oauth2-proxy --oidc-issuer-url="http://localhost:8080/realms/master" \
oauth2-proxy --redeem-url="http://localhost:8080/realms/master/protocol/openid-connect/token" \
oauth2-proxy --login-url="http://localhost:8080/realms/master/protocol/openid-connect/auth" \
oauth2-proxy --profile-url="http://localhost:8080/realms/master/protocol/openid-connect/userinfo" \
oauth2-proxy --validate-url="http://localhost:8080/realms/master/protocol/openid-connect/userinfo" \
oauth2-proxy --skip-provider-button=true \
oauth2-proxy --skip-auth-preflight=true \
oauth2-proxy --set-authorization-header=true \
oauth2-proxy --pass-user-headers=true \
oauth2-proxy --pass-authorization-header=true \
oauth2-proxy --pass-access-token=true \
oauth2-proxy --cookie-httponly=false \
oauth2-proxy --set-xauthrequest=true \
oauth2-proxy --pass-basic-auth=true \
oauth2-proxy --email-domain="*"




 ./oauth2-proxy \
oauth2-proxy --http-address=localhost:4180 \
oauth2-proxy --cookie-secure=false \
oauth2-proxy --cookie-secret=1234567890123456 \
oauth2-proxy --upstream="http://localhost:7007/api,http://localhost:3000/" \
oauth2-proxy --provider=keycloak \
oauth2-proxy --client-id=oauth2-proxy \
oauth2-proxy --client-secret=XjAzrZJ7enpo9bmlOXjL3RfMeGzBcZBF \
oauth2-proxy --oidc-issuer-url="http://localhost:8080/realms/master" \
oauth2-proxy --insecure-oidc-allow-unverified-email=true \
oauth2-proxy --redirect-url="http://localhost:4180/oauth2/callback" \
oauth2-proxy --oidc-issuer-url="http://localhost:8080/realms/master" \
oauth2-proxy --redeem-url="http://localhost:8080/realms/master/protocol/openid-connect/token" \
oauth2-proxy --login-url="http://localhost:8080/realms/master/protocol/openid-connect/auth" \
oauth2-proxy --profile-url="http://localhost:8080/realms/master/protocol/openid-connect/userinfo" \
oauth2-proxy --validate-url="http://localhost:8080/realms/master/protocol/openid-connect/userinfo" \
oauth2-proxy --skip-provider-button=true \
oauth2-proxy --set-authorization-header=true \
oauth2-proxy --pass-access-token=true \
oauth2-proxy --pass-basic-auth=false \
oauth2-proxy --set-xauthrequest=true \
oauth2-proxy --cookie-httponly=true \
oauth2-proxy --email-domain="*"



 ./oauth2-proxy \
oauth2-proxy --http-address=0.0.0.0:3000 \
oauth2-proxy --cookie-secure=false \
oauth2-proxy --cookie-secret=1234567890123456 \
oauth2-proxy --upstream="http://localhost:8080" \
oauth2-proxy --provider=keycloak-oidc \
oauth2-proxy --client-id=oauth2-proxy \
oauth2-proxy --client-secret=XjAzrZJ7enpo9bmlOXjL3RfMeGzBcZBF \
oauth2-proxy --oidc-issuer-url="http://localhost:9090/realms/master" \
oauth2-proxy --insecure-oidc-allow-unverified-email=true \
oauth2-proxy --redirect-url="http://localhost:4180/oauth2/callback" \
oauth2-proxy --oidc-issuer-url="http://localhost:9090/realms/master" \
oauth2-proxy --redeem-url="http://localhost:9090/realms/master/protocol/openid-connect/token" \
oauth2-proxy --login-url="http://localhost:9090/realms/master/protocol/openid-connect/auth" \
oauth2-proxy --profile-url="http://localhost:9090/realms/master/protocol/openid-connect/userinfo" \
oauth2-proxy --validate-url="http://localhost:9090/realms/master/protocol/openid-connect/userinfo" \
oauth2-proxy --skip-provider-button=true \
oauth2-proxy --email-domain="*" \
oauth2-proxy --set-xauthrequest=true

--email-domain=*
--pass-basic-auth=false
--pass-access-token=true
--set-xauthrequest=true
--skip-jwt-bearer-tokens=true
--set-authorization-header=true
--pass-authorization-header=true
--skip-auth-regex=^\/config\.json$
--skip-auth-regex=^\/favicon.*\.png$
--skip-auth-regex=^\/static\/
--skip-auth-regex=^\/$
--scope=openid email groups
--oidc-issuer-url=https://keycloak.example.org/auth/realms/kubernetes
--login-url=https://keycloak.example.org/auth/realms/kubernetes/protocol/openid-connect/auth
--redeem-url=https://keycloak.example.org/auth/realms/kubernetes/protocol/openid-connect/token
--validate-url=https://keycloak.example.org/auth/realms/kubernetes/protocol/openid-connect/userinfo
--keycloak-group=ipausers
