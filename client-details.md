
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
