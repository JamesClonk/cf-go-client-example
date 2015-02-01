# cf-go-client-example

This is example oauth client for CF.

Blog post: https://blog.starkandwayne.com/2014/11/11/simple-golang-oauth-client-for-cf

* add UAA client:
```
      cf-go-client-example:
        access-token-validity: 1209600
        authorities: scim.write,scim.read,cloud_controller.read,cloud_controller.write,password.write,uaa.admin,uaa.resource,cloud_controller.admin,billing.admin
        authorized-grant-types: authorization_code,client_credentials
        override: true
        redirect-uri: https://cf-go-client-example.10.244.0.34.xip.io/oauth2callback
        refresh-token-validity: 1209600
        scope: openid,cloud_controller.read,cloud_controller.write,password.write,console.admin,console.support
        secret: c1oudc0w
```
