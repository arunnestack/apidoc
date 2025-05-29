
## Client Details API
### GET
**Description:** Fetches details of a specific client by ID.
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{id}`
-  **Method:**  `GET`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205`

**Sample Response**

```json
{"id":205,"accountNo":"000000205","status":{"id":300,"code":"clientStatusType.active","value":"Active"},"active":true,"activationDate":[2023,6,9],"firstname":"Alka","displayName":"Alka ","mobileNo":"9033452134","dateOfBirth":[2007,5,12],"gender":{"id":24,"name":"Female","isActive":false,"mandatory":false},"clientType":{"isActive":false,"mandatory":false},"clientClassification":{"isActive":false,"mandatory":false},"salutation":{"isActive":false,"mandatory":false},"nationality":{"isActive":false,"mandatory":false},"education":{"isActive":false,"mandatory":false},"riskCategory":{"isActive":false,"mandatory":false},"officeId":5,"officeName":"Indore","timeline":{"submittedOnDate":[2023,6,9],"activatedOnDate":[2023,6,9]},"groups":[],"clientNonPersonDetails":{"constitution":{"isActive":false,"mandatory":false},"mainBusinessLine":{"isActive":false,"mandatory":false}},"isLocked":false,"isWorkflowEnabled":false,"maritalStatus":{"id":49,"name":"Unmarried","isActive":false,"mandatory":false},"isVerified":false,"isWorkflowEnableForBranch":false,"isMobileVerified":false,"officeHierarchy":".5."}
```

### PUT
**Description:** Update details of a specific client.
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{id}`
-  **Method:**  `PUT`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205`
**Sample Payload**
```json
{"firstname":"Alka","lastname":"Verma","active":true,"accountNo":"000000205","mobileNo":"9033452134","savingsProductId":null,"genderId":24,"clientNonPersonDetails":{},"maritalStatusId":49,"locale":"en","dateFormat":"dd MMMM yyyy","activationDate":"09 June 2023","dateOfBirth":"12 May 2007","submittedOnDate":"09 June 2023"}
```
**Sample Response**
```json
{"officeId":5,"clientId":205,"resourceId":205,"changes":{"lastname":"Verma"}}
```
<br>
<br>

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

<br>
<br>

## Client Address API
### GET
**Description:** Get list of address
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/addresses`
-  **Method:**  `GET`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/addresses`

**Sample Response**
```json
[{"addressId":13112,"addressLineOne":"638Q+CGR, Tiruvannamalai, Tamil Nadu 606601, India","districtData":{"districtId":644,"stateId":35,"isoDistrictCode":"AI","districtName":"Tiruvannamalai","talukaDatas":[],"cityDatas":[],"isWorkflowEnabled":false,"status":{"id":300,"code":"districtStatus.active","value":"ACTIVE"},"activationDate":[2021,8,27],"isWorkflowArchived":false},"stateData":{"stateId":35,"countryId":101,"isoStateCode":"TN","stateName":"Tamil Nadu","districtDatas":[],"isUt":false},"countryData":{"countryId":101,"isoCountryCode":"IN","countryName":"India"},"postalCode":"606601","noOfYrsAtCurrentResidence":0,"latitude":0,"longitude":0,"addressEntityData":[{"id":13112,"addressId":13112,"addressType":{"id":13,"name":"Permanent Address","isActive":true,"mandatory":false},"entityId":205,"entityType":{"id":1,"code":"addressEntityType.clients","value":"CLIENTS"},"isActive":true}]}]
```

### POST
**Description:** Create an address
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/addresses`
-  **Method:**  `POST`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/addresses`
**Sample Payload**
```json
{"addresses":[{"countryId":101,"stateId":21,"districtId":65,"talukaId":4,"addressRegionValueId":4,"postalCode":"606601","locale":"en","dateFormat":"dd MMMM yyyy","addressTypes":[74]}]}
```
**Sample Response**
```json
{"clientId":205,"resourceId":16905,"changes":{"resourceIds":[16905]}}
```

### DELETE
**Description:** Delete an address 
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/addresses/{addressID}`
-  **Method:**  `DELETE`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/addresses/16905`

**Sample Response**
```json
{"clientId":205,"resourceId":16905,"changes":{"entityType":1,"action":"delete"}}
```
