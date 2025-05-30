## Documents API
### GET
**Description:** Get list of documents
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/documents`
-  **Method:**  `GET`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/documents`

**Sample Response**
```json
[{"id":91365,"parentEntityType":"clients","parentEntityId":205,"name":"25287-location","fileName":"1748248004927.jpg","size":77700,"type":"image/jpeg","description":"voterid","reportIdentifier":0,"tagIdentifier":0,"status":{"id":1,"code":"INITIATED","value":"INITIATED"},"createdDate":1748248005000,"hasPassword":false}]
```

### POST
**Description:** Create a document
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/documents`
-  **Method:**  `POST`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/documents`
**Sample Payload Form**
```
name:test.jpg
file:base64data
description:voterid image
```
**Sample Response**
```json
{"officeId":5,"clientId":205,"resourceId":100330}
```

### DELETE
**Description:** Delete a document 
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/documents/{documentID}`
-  **Method:**  `DELETE`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/documents/91785`

**Sample Response**
```json
{"resourceId":91785,"changes":{},"resourceIdentifier":"91785"}
```
