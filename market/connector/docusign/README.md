Integrate eSignatures into your application in minutes. DocuSign's secure and award-winning eSignature makes requesting signatures, automating forms, and tracking documents directly from your app easy.

## Setup

1. Create a free DocuSign developer account: https://account-d.docusign.com/#/username
1. Create a new `application`: https://admindemo.docusign.com/authenticate?goTo=apiIntegratorKey
![create-app](doc/images/createAnApp.png)
1. Edit the created application:
![integration-key](doc/images/editApplication.png)
1. Open the `Definitions/Rest Clients` Editor in your Designer and select `DocuSign eSignature` client.
1. Copy the **Integration Key** from the docusign admin frontend into the Rest Clients property section value of `AUTH.integrationKey`
![integration-key](doc/images/copyIntegrationKeyAndSecret.png)
1. Scroll to **Authentication** choose `Authorization Code Grant`.
1. Click `Add Secrect Key` and copy the generated key into the Rest Clients property value called `AUTH.secretKey`
1. Scroll to the **Additional settings** section and add the `Redirect URI` from the Rest Clients property `AUTH.callback` into the docusign admin frontend.
![integration-key](doc/images/configureRedirectUri.png)
1. Save the changed application settings.