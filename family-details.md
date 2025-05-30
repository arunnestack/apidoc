## Family Details API
### GET
**Description:** Get list of familydetails
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/familydetails`
-  **Method:**  `GET`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/familydetails`

**Sample Response**
```json
[{"id":1767,"firstname":"ajay sonkar","dateOfBirth":"Jul 4, 2006","age":18,"relationship":{"id":27,"name":"Husband"},"gender":{"id":23,"name":"Male"},"isDependent":false,"isSeriousIllness":false,"isDeceased":false,"memberClientId":205,"displayName":"Alka Verma","accountNo":"000000205","isActive":true}]
```

### POST
**Description:** Create a familydetail
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/familydetails`
-  **Method:**  `POST`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/familydetails`
**Sample Payload**
```json
{"firstname":"Arun","dateOfBirth":"17 May 1994","age":31,"salutationId":108,"relationshipId":31,"genderId":23,"dateFormat":"dd MMMM yyyy","locale":"en"}
```
**Sample Response**
```json
{"officeId":5,"clientId":205,"resourceId":16965}
```

### DELETE
**Description:** Delete an familydetail 
-  **URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/{clientID}/familydetails/{documentID}`
-  **Method:**  `DELETE`
-  **Sample URL:**  `https://heylon.finflux.io/fineract-provider/api/v1/clients/205/familydetails/16965`

**Sample Response**
```json
{"officeId":5,"clientId":205,"resourceId":16965}
```
