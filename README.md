Spring SAML based integration with SSOCircle and Tableau
====================

### Dont forget to add unique SP at SSOCircle and in your code
### Update your Tableau servers landing URL at [landing.html](https://github.com/inbravo/spring-saml-tableau/blob/master/src/main/resources/templates/landing.html)
#### landing URL will show the Tableau data created by the test program at [tableau-restapi](https://github.com/inbravo/tableau-restapi). Please create the sample data at Tableau; which will be shown on landing page
### Download current SP metadata:
- Open web browser to the URL of the deployed application.
- Select Metadata information.
- Update method WebSecurityConfig.java/metadataGenerator() to add unique entityId
- Select first item from category Service providers, e.g. http://localhost:8080/saml/metadata
- Copy content of the Metadata textarea to your clipboard.

### Upload SP metadata to the IDP:
- Register yourself at www.ssocircle.com and login to the service.
- Select Metadata manager and click Add new Service Provider.
- Enter unique entityId in the FQDN field.
- Paste content of clipboard into the metadata information textarea.
- Store metadata by pressing the Submit button.
- Logout from the SSOCircle service.

---------





