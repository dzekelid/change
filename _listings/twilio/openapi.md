swagger: "2.0"
x-collection-name: Twilio
x-complete: 1
info:
  title: Twilio
  description: twilio-is-a-cloud-communications-infrastructure-as-a-serviceiaas-company-based-in-san-francisco-california--twilio-allows-software-developers-to-programmatically-make-and-receive-phone-calls-and-send-and-receive-text-messages-using-its-web-service-apis--twilios-services-are-accessed-over-http-and-are-billed-based-on-usage-
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/SIP/CredentialLists/{CLSid}:
    post:
      summary: Add SIP Credentials List
      description: Change the FriendlyName of the list
      operationId: change-the-friendlyname-of-the-list
      x-api-path-slug: accountsaccountsidsipcredentiallistsclsid-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: CLSid
        description: A 34 character string that uniquely identifies the credential
          list
      responses:
        200:
          description: OK
      tags:
      - SIP Credential Lists
  /Accounts/{AccountSid}/SIP/CredentialLists/{CLSid}/Credentials/{CredentialSid}:
    post:
      summary: Add To SIP Credentials List
      description: Change the password of a Credential record.nnIf the change is successful,
        Twilio will respond with the Credential record but will not include the password
        in the response.n
      operationId: change-the-password-of-a-credential-recordif-the-change-is-successful-twilio-will-respond-with-the-c
      x-api-path-slug: accountsaccountsidsipcredentiallistsclsidcredentialscredentialsid-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: CLSid
        description: A 34 character string that uniquely identifies the credential
          list
      - in: path
        name: CredentialSid
      responses:
        200:
          description: OK
      tags:
      - SIP Credential Lists
  /Accounts/{AccountSid}/SIP/IpAccessControlLists/{IpAccessControlListSid}/IpAddresses/{IpAddressSid}:
    post:
      summary: Add SIP IP Access Control List IP Address
      description: Change the description or IP address of a given IpAddress instance
        resource
      operationId: change-the-description-or-ip-address-of-a-given-ipaddress-instance-resource
      x-api-path-slug: accountsaccountsidsipipaccesscontrollistsipaccesscontrollistsidipaddressesipaddresssid-post
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: IpAccessControlListSid
        description: A 34 character string that uniquely identifies the SIP IP access
          control list
      - in: path
        name: IpAddressSid
        description: A 34 character string that uniquely identifies the SIP IP access
          control list
      responses:
        200:
          description: OK
      tags:
      - SIP IP Access Control Lists