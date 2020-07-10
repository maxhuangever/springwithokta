# Getting Started
It provides SSO feature, and supports authorization.

### Reference Documentation
https://developer.okta.com/blog/2017/03/16/spring-boot-saml

### code
 * resources/saml/idp.xml: 
   * for okta. Used to sign on okta. Due to proxy issue, metadata url can't be resolved, so download it into idp.xml.
   * Sign on url includes application data, which will be checked by Okta to see if you have permisson for the application.
   * In Okta, you need to assign the application to user. Otherwise, you will get message like `Sorry, you can't access Spring SAML because you are not assigned this app in Okta.`

 * resources/saml/keystore.jks: 
    * for https. use keytool to generate keystore.jks and its password is "secret".


