---
swagger: "2.0"
x-collection-name: Azure Cognitive Services
x-complete: 1
info:
  title: CognitiveServicesManagementClient
  description: cognitive-services-management-client
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.CognitiveServices/accounts/{accountName}:
    put:
      summary: Cognitive Services Accounts Create
      description: Create Cognitive Services Account. Accounts is a resource group
        wide resource type. It holds the keys for developer to access intelligent
        APIs. It's also the resource type for billing.
      operationId: CognitiveServicesAccounts_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-cognitiveservicesaccountsaccountname-put
      parameters:
      - in: path
        name: accountName
        description: The name of Cognitive Services account
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters to provide for the created account
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group within the users subscription
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Cognitive Service
    patch:
      summary: Cognitive Services Accounts Update
      description: Updates a Cognitive Services account
      operationId: CognitiveServicesAccounts_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-cognitiveservicesaccountsaccountname-patch
      parameters:
      - in: path
        name: accountName
        description: The name of Cognitive Services account
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters to provide for the created account
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group within the users subscription
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Cognitive Service
    delete:
      summary: Cognitive Services Accounts Delete
      description: Deletes a Cognitive Services account from the resource group.
      operationId: CognitiveServicesAccounts_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-cognitiveservicesaccountsaccountname-delete
      parameters:
      - in: path
        name: accountName
        description: The name of Cognitive Services account
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group within the users subscription
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Cognitive Service
    get:
      summary: Cognitive Services Accounts Get Properties
      description: Returns a Cognitive Services account specified by the parameters.
      operationId: CognitiveServicesAccounts_GetProperties
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-cognitiveservicesaccountsaccountname-get
      parameters:
      - in: path
        name: accountName
        description: The name of Cognitive Services account
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group within the users subscription
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Cognitive Service
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.CognitiveServices/accounts/{accountName}/listKeys
  : post:
      summary: Cognitive Services Accounts List Keys
      description: Lists the account keys for the specified Cognitive Services account.
      operationId: CognitiveServicesAccounts_ListKeys
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-cognitiveservicesaccountsaccountnamelistkeys-post
      parameters:
      - in: path
        name: accountName
        description: The name of Cognitive Services account
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group within the users subscription
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Cognitive Service
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.CognitiveServices/accounts/{accountName}/regenerateKey
  : post:
      summary: Cognitive Services Accounts Regenerate Key
      description: Regenerates the specified account key for the specified Cognitive
        Services account.
      operationId: CognitiveServicesAccounts_RegenerateKey
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-cognitiveservicesaccountsaccountnameregeneratekey-post
      parameters:
      - in: path
        name: accountName
        description: The name of Cognitive Services account
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: regenerate key parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group within the users subscription
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Cognitive Service
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.CognitiveServices/accounts/{accountName}/skus
  : get:
      summary: Cognitive Services Accounts List Skus
      description: List available SKUs for the requested Cognitive Services account
      operationId: CognitiveServicesAccounts_ListSkus
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-cognitiveservicesaccountsaccountnameskus-get
      parameters:
      - in: path
        name: accountName
        description: The name of Cognitive Services account
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group within the users subscription
      responses:
        200:
          description: OK
      tags:
      - Machine Learning
      - Cognitive Service
---