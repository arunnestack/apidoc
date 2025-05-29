## Client Identifiers API
### GET
**Description:** Get list of identifiers
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/identifiers`
-  **Method:**  `GET`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/identifiers`

**Sample Response**
```json
[{"id":25209,"clientId":205,"documentType":{"id":4,"name":"Any Other Id Type","isActive":false,"mandatory":false},"documentKey":"205","description":"foWA58LTS96nI3_hm2HoQW:APA91bEfa4zRY4sSg1pwD6D2cRPuQXqYYtF0FYRYgmLHmzQ490E78yiCJ2EboNE2nDJYKgnn7SgzxmYI30NRDv1FkQr8wwp6o6EtWxWIxd5LTe9Xga2mh-0","status":"clientIdentifierStatusType.active","subCategoryType":{"isActive":false,"mandatory":false},"clientIdentifierVerifiedDetailsData":{"isVerified":false},"proof":[]},{"id":67859,"clientId":205,"documentType":{"id":25,"name":"Voter Id","isActive":false,"mandatory":false,"systemIdentifier":"VID"},"documentKey":"ABC1234567","description":"Alka","status":"clientIdentifierStatusType.active","subCategoryType":{"isActive":false,"mandatory":false},"clientIdentifierVerifiedDetailsData":{"isVerified":false},"proof":[]}]
```

### POST
**Description:** Create an identifier
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/identifiers`
-  **Method:**  `POST`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/identifiers`
**Sample Payload**
```json
{"documentTypeId":25,"status":200,"documentKey":"ABC1234567","locale":"en","dateFormat":"dd MMMM yyyy"}
```
**Sample Response**
```json
{"officeId":5,"clientId":205,"resourceId":100330}
```

### PUT
**Description:** Update an identifier
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/identifiers/{identifierID}`
-  **Method:**  `PUT`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/identifiers/100330`
**Sample Payload**
```json
{"documentTypeId":25,"status":200,"documentKey":"ABC1234567","locale":"en","dateFormat":"dd MMMM yyyy"}
```
**Sample Response**
```json
{"officeId":5,"clientId":205,"resourceId":100330}
```


### DELETE
**Description:** Delete an identifier 
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/identifiers/{identifierID}`
-  **Method:**  `DELETE`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/identifiers/67859`

**Sample Response**
```json
{"officeId":5,"clientId":205,"resourceId":67859}
```
